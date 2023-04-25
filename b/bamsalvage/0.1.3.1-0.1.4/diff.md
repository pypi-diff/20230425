# Comparing `tmp/bamsalvage-0.1.3.1-py3-none-any.whl.zip` & `tmp/bamsalvage-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9984 bytes, number of entries: 7
+Zip file size: 10370 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      294 b- defN 20-Feb-02 00:00 bamsalvage/__init__.py
--rwxr-xr-x  2.0 unx    24505 b- defN 20-Feb-02 00:00 bamsalvage/_bamsalvage.py
-?rw-r--r--  2.0 unx     1919 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      584 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/RECORD
-7 files, 28507 bytes uncompressed, 8944 bytes compressed:  68.6%
+-rwxr-xr-x  2.0 unx    25966 b- defN 20-Feb-02 00:00 bamsalvage/_bamsalvage.py
+?rw-r--r--  2.0 unx     1938 b- defN 20-Feb-02 00:00 bamsalvage-0.1.4.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 bamsalvage-0.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 bamsalvage-0.1.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 bamsalvage-0.1.4.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      574 b- defN 20-Feb-02 00:00 bamsalvage-0.1.4.dist-info/RECORD
+7 files, 29977 bytes uncompressed, 9350 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: bamsalvage/__init__.py
 Comment: 
 
 Filename: bamsalvage/_bamsalvage.py
 Comment: 
 
-Filename: bamsalvage-0.1.3.1.dist-info/METADATA
+Filename: bamsalvage-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: bamsalvage-0.1.3.1.dist-info/WHEEL
+Filename: bamsalvage-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: bamsalvage-0.1.3.1.dist-info/entry_points.txt
+Filename: bamsalvage-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: bamsalvage-0.1.3.1.dist-info/licenses/LICENSE
+Filename: bamsalvage-0.1.4.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: bamsalvage-0.1.3.1.dist-info/RECORD
+Filename: bamsalvage-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bamsalvage/__init__.py

```diff
@@ -3,12 +3,12 @@
 #print('BAMSALVAGE: Imported {}'.format(__file__))
 
 from bamsalvage._bamsalvage import *
 
 try:
     __version__ = version(__name__)
 except Exception:
-    __version__="0.1.2"
+    __version__="0.1.4"
     pass
 
 # from _bamsalvage import *
```

## bamsalvage/_bamsalvage.py

```diff
@@ -1,77 +1,95 @@
 import os, sys, re, io
 import argparse, struct
-import mgzip, gzip
+import mgzip
 import zlib, logging, json
 import numba
 import numpy as np
 
-
+# Error handling
 class BAMException(Exception):
     """Exception for BAM decoding
     """
     NO_BAM_FILE = 0
     BLOCK_CORRUPTED = 1
     EXCEED_EXPECTED_SIZE = 2
     INCORRECT_MAGIC_NUMBER = 3
     INCORRECT_GZIP_MAGIC_NUMBER = 4
     BUFFER_TERMINATED = 5
     INCONSISTENT_CHECKSUM = 6
     INCONSISTENT_BLOCK_SIZE = 7
     DECOMPRESSION_FAILURE = 8
+    OUT_OF_RANGE_VARIABLES = 9
     __KIND = ['This is not BAM file', 
               'Block was corrupted', 'Expected buffer size overflow',
               'Incorrect magic number', 'Incorrect GZIP magic number', 
               'Reached the end of file', 'Inconsistent CRC32 checksum',
               'Decompressed buffer size was inconsisted with expected',
-              "Failed to decompress"]
+              "Failed to decompress", 'Variables are out of range']
     def __init__(self, kind:int, message:str=''):
         super(BAMException, self).__init__(message)
         if kind < 0 or kind > len(BAMException.__KIND):
             kind = -1
         self.__kind = kind
     def __str__(self):
-        if self.__kind < 0 or self.__kind >= len(BAMException.__KIND):
-            estr = 'unknown error'
-        else:
-            estr = BAMException.__KIND[self.__kind]
-        return '{} {}'.format(super().__str__(), estr)
+        return '{} {}'.format(super().__str__(), BAMException.resolve_error_code(self.__kind))
+    @classmethod
+    def resolve_error_code(cls, kind):
+        if 0 <= kind < len(cls.__KIND):
+            return cls.__KIND[kind]
+        if kind == -1:
+            return 'unclassified error in reading a block'
+        if kind == -2:
+            return 'parameters inconsitency'
+        if kind == -3:
+            return ''
+        return 'Unknown error'
     kind = property(lambda s:s.__kind)
+
+# Optimized functions using Numba
 @numba.njit(cache=True)
 def convert_bytes_to_seq(buffer:bytes, start:int, l_seq:int, text:bytearray):
+    """Convert 4-byte encoded sequence to ASCII
+    """
     bases = [61, 65, 67, 77, 71, 82, 83, 86, 84, 87, 89, 72, 75, 68, 66, 78] # '=ACMGRSVTWYHKDBN'
     j = 0
     end = start + (l_seq + 1) // 2
     for i in range(start, end):
         b = buffer[i]
         text[j] = bases[b >> 4]
         if j + 1 >= l_seq: break
         text[j+1] = bases[b & 15]
         j += 2
 @numba.njit(cache=True)
 def convert_bytes_to_qual(buffer:bytes, start:int, l_seq:int, text:bytearray):
-    j = 0
-    end = start + l_seq
-    for i in range(start, end):
-        b = buffer[i]
-        text[i-start] = 33 + b
+    """Convert byte array into QUAL sequence"""
+    for i in range(l_seq):
+        text[i] = min(33 + buffer[start+i], 127)
 
 @numba.njit(cache=True)
 def scan_block_header(buffer:bytes, start:numba.int64)->numba.int64:
-    le_I = np.dtype('uint32')
-    le_i = np.dtype('int32')
+    """Scan magic number and signature bytes int data block"""
+    # le_I = np.uint32
+    # le_i = np.int32
     for i in range(start, len(buffer)-36):
-        block_size = np.frombuffer(buffer[i:i+4], dtype=le_I)[0]
-        refid = np.frombuffer(buffer[i+4:i+8], dtype=le_i)[0]
+        block_size = np.frombuffer(buffer[i:i+4], dtype=np.uint32)[0]
+        refid = np.frombuffer(buffer[i+4:i+8], dtype=np.int32)[0]
         l_read_name = np.frombuffer(buffer[i+12:i+16], dtype=np.uint8)[0]
-        l_seq = np.frombuffer(buffer[i+20:i+24], dtype=le_I)[0]
+        l_seq = np.frombuffer(buffer[i+20:i+24], dtype=np.uint32)[0]
         if 0 <= l_seq < block_size * 3 // 2 and l_read_name > 4 and -1 <= refid < 200 and block_size + start < len(buffer):
             return i
     return -1
 
+# @numba.njit('i8(u8[:], u8)', cache=True)
+# def _find_byte(bytes, byte):
+#     for i in range(bytes.size):
+#         if bytes[i] == byte:
+#             return i
+#     return len(bytes)
+
 def _get_logger(name=None, stdout=True, logfile=None):
     if name is None:
         name = sys._getframe().f_code.co_name
         pass
     
     logger = logging.getLogger(name)
     # set logging
@@ -87,21 +105,14 @@
         stdout = True
     if stdout:
         _set_log_handler(logger, logging.StreamHandler())
     # logger.setLevel(logging.ERROR)
     logger.propagate = False
     return logger
 
-@numba.njit('i8(u8[:], u8)', cache=True)
-def _find_byte(bytes, byte):
-    for i in range(bytes.size):
-        if bytes[i] == byte:
-            return i
-    return len(bytes)
-
 def scan_next_block(handler, **kwargs):
     """Read BGZF block
 
      ID1   0-0 u8 = 31 
      ID2   1-1 u8 = 139
      CM    2-2 u8 = 8
      FLG   3-3 u8 = 4
@@ -151,39 +162,14 @@
         _skip_bytes = xlen - 6
         handler.read(_skip_bytes)
     if len(buf) < xlen:
         raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot load gzipped block AT {} '.format(current_pos))
     compressed_data_size = block_size - xlen - 19
     return decompress_and_validate(handler, compressed_data_size)
 
-def decompress_and_validate(handler, compressed_data_size):
-    current_pos = handler.tell()
-    cdata = handler.read(compressed_data_size)
-
-    decobj = zlib.decompressobj(-15) # no header
-    try:
-        decompressed = decobj.decompress(cdata) + decobj.flush()
-    except Exception as e:
-        raise BAMException(BAMException.DECOMPRESSION_FAILURE, '{} AT {} '.format(str(e), current_pos))
-
-    buf = handler.read(8)
-    if len(buf) < 8:
-        raise BAMException(BAMException.BUFFER_TERMINATED, ' AT {} '.format(current_pos))
-    crc32, input_size = struct.unpack('<II', buf)
-    if input_size == len(decompressed):
-        crc32_calc = zlib.crc32(decompressed)
-        if crc32_calc != crc32:            
-            raise BAMException(BAMException.INCONSISTENT_CHECKSUM, 'CRC is {:x} , not {:x} AT {} '.format(crc32_calc, crc32, current_pos))
-        return decompressed
-    else:
-        # sys.stderr.write(f'inconsistent size of decompressed buffer {expected_size} / {len(data)}\n')
-        raise BAMException(BAMException.INCONSISTENT_BLOCK_SIZE, 
-                           'inconsistent zlib size expected={}, decompressed={} AT {} '.format(
-                                input_size, len(decompressed), current_pos))
-    return decompressed
     
 def read_next_block(handler, **kwargs):
     """Read BGZF block, block corruption is not assumed.
 
     Args:
         handler (_io.TextIOWrapper): File handler
 
@@ -202,32 +188,52 @@
     buf = handler.read(10)
     values = struct.unpack('<BBIBBH', buf)
     xlen = values[-1]
     buf = handler.read(xlen)
     si1, si2, slen, bsize = struct.unpack('<BBHH', buf[0:6])
     if si1 != 66 or si2 != 67:
         raise BAMException(BAMException.INCORRECT_GZIP_MAGIC_NUMBER, 'SI1={}, SI2={} is different from 66 and 67'.format(si1, si2))
-    decobj = zlib.decompressobj(-15) # no header
     return decompress_and_validate(handler, bsize - xlen - 19)
-    # compressed = handler.read(bsize - xlen - 19)
-    # expected_crc, expected_size = struct.unpack('<II', handler.read(8))
-    # decompressed = decobj.decompress(compressed) + decobj.flush()
-
-    # # CRC check
-    # crc_calc = struct.unpack('<I', decompressed[0:4])[0]#zlib.crc32(data))[0]
-
-    # if expected_size == len(decompressed):
-    #     calculated_crc32 = zlib.crc32(decompressed)
-    #     if calculated_crc32 != expected_crc:
-    #         raise BAMException(BAMException.INCONSISTENT_CHECKSUM, 'CRC is {:x} , not {:x}'.format(calculated_crc, expected_crc))
-    #     return decompressed
-    # else:
-    #     raise BAMException(BAMException.INCONSISTENT_BLOCK_SIZE, 
-    #                        'inconsistent zlib size expected={}, decompressed={}'.format(
-    #                             expected_size, len(decompressed)))
+
+def decompress_and_validate(handler, compressed_data_size):
+    """Read data block and validate BGZF block. Common routine among read_next_block and scan_next_block functions.
+
+    Args:
+        handler (stream): Stream handler
+        compressed_data_size (_type_): _description_
+
+    Raises:
+        BAMException: Corrupted block detected
+
+    Returns:
+        byte array : data block
+    """
+    current_pos = handler.tell()
+    cdata = handler.read(compressed_data_size)
+
+    decobj = zlib.decompressobj(-15) # no header
+    try:
+        decompressed = decobj.decompress(cdata) + decobj.flush()
+    except Exception as e:
+        raise BAMException(BAMException.DECOMPRESSION_FAILURE, '{} AT {} '.format(str(e), current_pos))
+
+    buf = handler.read(8)
+    if len(buf) < 8:
+        raise BAMException(BAMException.BUFFER_TERMINATED, ' AT {} '.format(current_pos))
+    crc32, input_size = struct.unpack('<II', buf)
+    if input_size == len(decompressed):
+        crc32_calc = zlib.crc32(decompressed)
+        if crc32_calc != crc32:            
+            raise BAMException(BAMException.INCONSISTENT_CHECKSUM, 'CRC is {:x} , not {:x} AT {} '.format(crc32_calc, crc32, current_pos))
+        return decompressed
+    else:
+        # sys.stderr.write(f'inconsistent size of decompressed buffer {expected_size} / {len(data)}\n')
+        raise BAMException(BAMException.INCONSISTENT_BLOCK_SIZE, 
+                           'inconsistent zlib size expected={}, decompressed={} AT {} '.format(
+                                input_size, len(decompressed), current_pos))
 
 def retrieve_fastq_from_bam(filename_bam:str, filename_fastq:str, **kwargs)->dict:
     """Retrieving fastq sequences from BAM file
 
     Args:
         filename_bam (str): BAM filename
         filename_fastq (str): Fastq filename 
@@ -248,110 +254,118 @@
         ostr = sys.stdout
     elif filename_fastq.endswith('.gz'):                                                                                                                                                   
         n_threads = kwargs.get('threads', 4)
         ostr = io.TextIOWrapper(mgzip.open(filename_fastq, 'wb', thread=n_threads))
     else:
         ostr = open(filename_fastq, 'w')
         
-    if seek_pos > 0:
-        logger.info('seek at {:.0}'.format(seek_pos * filesize))
-        fi.seek(int(seek_pos * filesize))
-    
     filesize = os.path.getsize(filename_bam)
+    tracking_data = []
     # TRACE_ID_READING = 0
     # TRACE_ID_ALIGNMENT = 1
     # tracing_situations = [TRACE_ID_READING, TRACE_ID_ALIGNMENT]
     # tracing_ptr = [-1] * (max(tracing_situations) + 1)
 
     MAXIMUM_BLOCK_SIZE = 1024 * 1024
     MINIMUM_READ_NAME = 2
     with open(filename_bam, 'rb') as fi:
+        if seek_pos > 0:
+            logger.info('seek at {}'.format(seek_pos))
+            fi.seek(min(seek_pos, filesize))
+
         references = []
         n_blocks = 0
-        n_corrupted_blocks = 0
+        pos = 0
+        # n_corrupted_blocks = 0
         n_malformed_gzip_blocks = 0
         n_unaligned_blocks = 0
         
         # read header
-        file_ptr = 0 # pointer of file for backtracking
-        try:
-            n_blocks += 1
-            data = read_next_block(fi)
-            if data[0:4] != b'BAM\1':
-                logger.warning('BAM header lost\n')
-                raise Exception('the file is not BAM')
-            l_text = struct.unpack('<I', data[4:8])[0]
-            while l_text + 12 > len(data):
-                logger.info('reading remant header {}/{}\n'.format(len(data), l_text))
+        if seek_pos == 0: # read header if the process starts from the top
+            file_ptr = 0 # pointer of file for backtracking
+            try:
                 n_blocks += 1
-                data += scan_next_block(fi)
-            text_ = data[8:8+l_text].decode('latin-1')
-            pos = 8 + l_text
-            # load references
-            n_ref = struct.unpack('<I', data[pos:pos+4])[0]
-            logger.info(f'references : {n_ref}')
-            pos += 4
-            for i in range(n_ref):
-                l_name = struct.unpack('<I', data[pos:pos+4])[0]
-                pos += 4
-                name = data[pos:pos + l_name].decode('latin-1')[:-1]
-                pos += l_name
-                l_ref = struct.unpack('<I', data[pos:pos+4])[0]
-                references.append((name, l_ref))
-                # logger.info('@SQ\t{}\tLN:{}'.format(name, l_ref))
-                pos += 4
-                if pos > len(data): #
-                    # logger.info('extend header block {} / {}'.format(pos, len(data)))
+                data = read_next_block(fi)
+                if data[0:4] != b'BAM\1':
+                    logger.warning('BAM header lost\n')
+                    raise Exception('the file is not BAM')
+                l_text = struct.unpack('<I', data[4:8])[0]
+                while l_text + 12 > len(data):
+                    logger.info('reading remant header {}/{}\n'.format(len(data), l_text))
                     n_blocks += 1
                     data += scan_next_block(fi)
-            info['references'] = references
-        except BAMException as e:
-            if e.kind == BAMException.BUFFER_TERMINATED: # end of file
-                logger.warning('no header and file terminated')
-                return
-            else:
-                logger.warning(str(e))
-            # logger.warning('header was corrupted, skip header blocks {}'.format(str(e)))
-            n_malformed_gzip_blocks += 1
-        except Exception as e:
-            # if not force_continuation:
-            #     raise
-            logger.warning('header was corrupted, skip header blocks')
-            n_malformed_gzip_blocks += 1
-            raise
+                text_ = data[8:8+l_text].decode('latin-1')
+                pos = 8 + l_text
+                # load references
+                n_ref = struct.unpack('<I', data[pos:pos+4])[0]
+                logger.info(f'references : {n_ref}')
+                pos += 4
+                for i in range(n_ref):
+                    l_name = struct.unpack('<I', data[pos:pos+4])[0]
+                    pos += 4
+                    name = data[pos:pos + l_name].decode('latin-1')[:-1]
+                    pos += l_name
+                    l_ref = struct.unpack('<I', data[pos:pos+4])[0]
+                    references.append((name, l_ref))
+                    # logger.info('@SQ\t{}\tLN:{}'.format(name, l_ref))
+                    pos += 4
+                    if pos > len(data): #
+                        # logger.info('extend header block {} / {}'.format(pos, len(data)))
+                        n_blocks += 1
+                        data += scan_next_block(fi)
+                info['references'] = references
+            except BAMException as e:
+                if e.kind == BAMException.BUFFER_TERMINATED: # end of file
+                    logger.warning('no header and file terminated')
+                    return
+                else:
+                    logger.warning(str(e))
+                tracking_data.append([e.kind, file_ptr])
+                # logger.warning('header was corrupted, skip header blocks {}'.format(str(e)))
+                n_malformed_gzip_blocks += 1
+            except Exception as e:
+                # if not force_continuation:
+                #     raise
+                tracking_data.append([-2, file_ptr])
+                logger.warning('header was corrupted, skip header blocks')
+                n_malformed_gzip_blocks += 1
+                raise
 
         # alignment section
         n_seqs = 0
         total_bases = 0
         keep_running = True
-        scanning = False
+#        scanning = False
         data = []
-        scanning = True
+        # scanning = True
         
         # scanning = True
         while keep_running:
             # first block after buffer flushing
             file_ptr = fi.tell()
             if file_ptr >= filesize: # check position is in the file size
+                tracking_data.append([BAMException.BUFFER_TERMINATED, file_ptr]) # end
                 break
             try:
                 n_blocks += 1
                 if pos == 0:
                     data = scan_next_block(fi)
                 else:
                     data = read_next_block(fi)
             except BAMException as e:
                 logger.warning(str(e))
                 n_malformed_gzip_blocks += 1
-                scanning = True
+                tracking_data.append([e.kind, file_ptr])
+                # scanning = True
                 pos = 0
                 continue
             except:
                 n_malformed_gzip_blocks += 1
-                scanning = True
+                tracking_data.append([-2, file_ptr])
+                # scanning = True
                 raise
             pos = 0
             
             # if scanning:
             #     sys.stderr.write('\033[Kscanning {}, {}, {}\r\n'.format(n_blocks, len(data), pos))
             #     pos_scanned = scan_block_header(data, pos)
             #     if pos_scanned >= 0:
@@ -360,20 +374,35 @@
             #     else:
             #         continue
                 
             # read data until the end of block
             while pos < len(data):
                 file_ptr = fi.tell()
                 if file_ptr >= filesize: # check position is in the file size
+                    tracking_data.append([BAMException.BUFFER_TERMINATED, file_ptr])
                     break
                 if pos > 0:
                     data = data[pos:]
                     pos = 0
+                if len(data) < 36: # buffer is empty
+                    sys.stderr.write(f'\033[Kbuffer size below 36 AT {file_ptr}\n')
+                    data = []
+                    pos = 0
+                    break
                 block_size, refid, mappos, l_read_name, mapq, bai_bin, n_cigar_op, flag, l_seq, next_refid, next_pos, tlen \
                     = struct.unpack('<IiiBBHHHIiii', data[pos:pos + 36])
+
+                # assert variable range
+                if l_seq >= block_size * 3 // 2 or l_read_name < 5 or refid < -2 or refid >= len(references): # invalid block
+                    n_unaligned_blocks += 1
+                    tracking_data.append([BAMException.OUT_OF_RANGE_VARIABLES, file_ptr])
+                    data = []
+                    pos = 0
+                    break
+
                 ptr_block_start = pos + 4 # start position of data field
                 
                 # print(block_size, l_read_name, l_seq)
                 if block_size > MAXIMUM_BLOCK_SIZE or l_read_name < MINIMUM_READ_NAME:
                     block_size = 0
                 else:
                     # read data block
@@ -381,37 +410,30 @@
                         # print(block_size + ptr_block_start, len(data), fi.tell())
                         # logger.info('extending alignment block to {} (current {})'.format(block_size, len(data) - pos))
                         try:
                             n_blocks += 1
                             data += read_next_block(fi)
                         except BAMException as e:
                             # tracing_ptr[TRACE_ID_READING] = file_ptr
+                            tracking_data.append([e.kind, file_ptr])
                             n_malformed_gzip_blocks += 1
                             # sys.stderr.write(str(e) + '\n')
                             logger.warning('\033[Kfailed to loading : {}'.format(str(e)))
                             data = []
                             break
                         except Exception as e:
+                            tracking_data.append([-1, file_ptr])
                             raise
                     if len(data) == 0: # skip blocks
-                        scanning = True
+                        # scanning = True
                         break
                     
-                # assert variable range
-                if l_seq >= block_size * 3 // 2 or l_read_name < 5 or refid < -2 or refid >= len(references): # invalid block
-                    n_unaligned_blocks += 1
-                    # tracing_ptr[TRACE_ID_ALIGNMENT] = file_ptr
-                    scanning = True
-                    data = []
-                    pos = 0
-                    break
-                
                 # logger.info(f'pos={pos}/{len(data)}\tname={l_read_name}, l_seq={l_seq}, refid={refid}, pos={mappos}, MAPQ={mapq}, bin={bai_bin}, n_cigar={n_cigar_op}, flag={flag}')
                 #bases = '=ACMGRSVTWYHKDBN'
-                scanning = False
+                # scanning = False
                 pos += 36
                 seqid = data[pos:pos + l_read_name].decode('latin-1')[:-1]
                 pos += l_read_name + n_cigar_op * 4
                 n_seqs += 1
                 total_bases += l_seq
 
                 if ostr:
@@ -433,16 +455,16 @@
                         pos += l_seq
                 pos = ptr_block_start + block_size
                 if n_seqs % 1000 == 0:
                     if limit > 0 and n_seqs >= limit:
                         keep_running = False
                         break
                     percentage = fi.tell() / filesize * 100.0
-                    sys.stderr.write('\033[K {:.1f}% {}\t{} kreads\t{} blocks ({},{} corrupted)\r'.format(
-                        percentage, seqid[:16], n_seqs // 1000, n_blocks, n_malformed_gzip_blocks, n_unaligned_blocks))
+                    sys.stderr.write('\033[K {:.1f}% {}\t{} kreads\t{} blocks ({} corrupted)\r'.format(
+                        percentage, seqid[:16], n_seqs // 1000, n_blocks, len(tracking_data)))
 
                 block_end = ptr_block_start + block_size
 
                 # auxiliary data 
                 if True: 
                     pos = block_end
                     continue
@@ -506,14 +528,15 @@
     sys.stderr.write('\033[K\r')
     info['n_seqs'] = n_seqs
     info['n_blocks'] = n_blocks
     info['n_corrupted'] = n_malformed_gzip_blocks + n_unaligned_blocks
     info['n_malformed_gzip_blocks'] =  n_malformed_gzip_blocks
     info['n_unaligned_blocks'] = n_unaligned_blocks
     info['total_bases'] = total_bases
+    info['error.log'] = tracking_data
 
     # info['traces'] = {'':tracking
     # info['tracing'] = {
     #     'reading':tracing_ptr[TRACE_ID_READING],
     #     'alignment':tracing_ptr[TRACE_ID_ALIGNMENT]}
 
     return info
@@ -588,14 +611,22 @@
             elif fasta:
                 filename_out = os.path.join(outdir, title + '.fa')
             else:
                 filename_out = os.path.join(outdir, title + '.fastq')
             if (not stdout_mode) and gzipped:
                 filename_out += '.gz'
             finfo = retrieve_fastq_from_bam(filename, filename_out, logger=logger, limit=limit, threads=n_threads, fileseek=seek_pos)
+            tracking_data = finfo.pop('error.log', [])
+            filename_log = os.path.join(outdir, '.{}.log'.format(os.path.basename(filename)))
+            with open(filename_log, 'w') as fo:
+                fo.write('#filename={}\n'.format(filename))
+                fo.write('#filesize={}\n'.format(os.path.getsize(filename)))
+                fo.write('#code\tfile_pos\tkind\n')
+                for kind, pos in tracking_data:
+                    fo.write('{}\t{}\t{}\n'.format(kind, pos, BAMException.resolve_error_code(kind)))
             info['files'].append(finfo)
     if outdir is None:
         print(json.dumps(info))
     else:
         fn_info = os.path.join(outdir, 'run.info')
         with open(fn_info, 'w') as fo:
             json.dump(info, fo, indent=2)
```

## Comparing `bamsalvage-0.1.3.1.dist-info/METADATA` & `bamsalvage-0.1.4.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: bamsalvage
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: Sequence salvaging script from corrupted BAM files
 Project-URL: Homepage, https://pypi.org/project/bamsalvage/
 Author-email: Example Author <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: mgzip
 Requires-Dist: numba
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # bamsalvage
 ## INTRODUCTION
 bamsalvage is a tools to recover sequence reads as much as possible from possibly corrupted BAM files.
```

## Comparing `bamsalvage-0.1.3.1.dist-info/licenses/LICENSE` & `bamsalvage-0.1.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

