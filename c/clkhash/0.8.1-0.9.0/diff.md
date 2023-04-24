# Comparing `tmp/clkhash-0.8.1.tar.gz` & `tmp/clkhash-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clkhash-0.8.1.tar", last modified: Fri Jan 19 04:43:49 2018, max compression
+gzip compressed data, was "dist/clkhash-0.9.0.tar", last modified: Thu Feb 15 23:01:27 2018, max compression
```

## Comparing `clkhash-0.8.1.tar` & `clkhash-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-01-19 04:43:49.000000 clkhash-0.8.1/
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash/
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash/data/
--rw-r--r--   0 brian     (1000) brian     (1000)   695430 2017-07-17 23:24:38.000000 clkhash-0.8.1/clkhash/data/CSV_Database_of_Last_Names.csv
--rw-r--r--   0 brian     (1000) brian     (1000)    87350 2017-07-17 23:24:38.000000 clkhash-0.8.1/clkhash/data/female-first-names.csv
--rw-r--r--   0 brian     (1000) brian     (1000)  6248044 2017-07-17 23:24:38.000000 clkhash-0.8.1/clkhash/data/first-name-counts-by-year.csv
--rw-r--r--   0 brian     (1000) brian     (1000)    65929 2017-07-17 23:24:38.000000 clkhash-0.8.1/clkhash/data/male-first-names.csv
--rw-r--r--   0 brian     (1000) brian     (1000)      283 2017-10-16 05:23:18.000000 clkhash-0.8.1/clkhash/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1000)     1091 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/benchmark.py
--rw-r--r--   0 brian     (1000) brian     (1000)     4847 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/bloomfilter.py
--rw-r--r--   0 brian     (1000) brian     (1000)     9640 2017-12-14 03:56:35.000000 clkhash-0.8.1/clkhash/cli.py
--rw-r--r--   0 brian     (1000) brian     (1000)     4504 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/clk.py
--rw-r--r--   0 brian     (1000) brian     (1000)     3151 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/identifier_types.py
--rw-r--r--   0 brian     (1000) brian     (1000)     7582 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/key_derivation.py
--rw-r--r--   0 brian     (1000) brian     (1000)     5165 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/randomnames.py
--rw-r--r--   0 brian     (1000) brian     (1000)     1107 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/schema.py
--rw-r--r--   0 brian     (1000) brian     (1000)     1518 2018-01-09 03:14:44.000000 clkhash-0.8.1/clkhash/tokenizer.py
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)      253 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash.egg-info/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      583 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash.egg-info/SOURCES.txt
--rw-r--r--   0 brian     (1000) brian     (1000)        1 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash.egg-info/dependency_links.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       45 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash.egg-info/entry_points.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       99 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash.egg-info/requires.txt
--rw-r--r--   0 brian     (1000) brian     (1000)        8 2018-01-19 04:43:49.000000 clkhash-0.8.1/clkhash.egg-info/top_level.txt
--rw-r--r--   0 brian     (1000) brian     (1000)     2403 2018-01-09 03:14:44.000000 clkhash-0.8.1/README.md
--rw-r--r--   0 brian     (1000) brian     (1000)       67 2018-01-19 04:43:49.000000 clkhash-0.8.1/setup.cfg
--rw-r--r--   0 brian     (1000) brian     (1000)      701 2018-01-19 04:43:16.000000 clkhash-0.8.1/setup.py
--rw-r--r--   0 brian     (1000) brian     (1000)      253 2018-01-19 04:43:49.000000 clkhash-0.8.1/PKG-INFO
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-02-15 23:01:27.000000 clkhash-0.9.0/
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash/
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash/data/
+-rw-r--r--   0 brian     (1000) brian     (1000)   695430 2017-07-17 23:24:38.000000 clkhash-0.9.0/clkhash/data/CSV_Database_of_Last_Names.csv
+-rw-r--r--   0 brian     (1000) brian     (1000)    87350 2017-07-17 23:24:38.000000 clkhash-0.9.0/clkhash/data/female-first-names.csv
+-rw-r--r--   0 brian     (1000) brian     (1000)  6248044 2017-07-17 23:24:38.000000 clkhash-0.9.0/clkhash/data/first-name-counts-by-year.csv
+-rw-r--r--   0 brian     (1000) brian     (1000)    65929 2017-07-17 23:24:38.000000 clkhash-0.9.0/clkhash/data/male-first-names.csv
+-rw-r--r--   0 brian     (1000) brian     (1000)      283 2017-10-16 05:23:18.000000 clkhash-0.9.0/clkhash/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     1091 2018-01-09 03:14:44.000000 clkhash-0.9.0/clkhash/benchmark.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     6288 2018-02-15 04:22:40.000000 clkhash-0.9.0/clkhash/bloomfilter.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     9732 2018-02-15 04:22:40.000000 clkhash-0.9.0/clkhash/cli.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     4937 2018-02-15 23:00:15.000000 clkhash-0.9.0/clkhash/clk.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     3964 2018-02-15 04:22:40.000000 clkhash-0.9.0/clkhash/identifier_types.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     7582 2018-01-09 03:14:44.000000 clkhash-0.9.0/clkhash/key_derivation.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     5165 2018-01-09 03:14:44.000000 clkhash-0.9.0/clkhash/randomnames.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     1107 2018-01-09 03:14:44.000000 clkhash-0.9.0/clkhash/schema.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     1518 2018-01-09 03:14:44.000000 clkhash-0.9.0/clkhash/tokenizer.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)      253 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      583 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)        1 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       45 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash.egg-info/entry_points.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)      128 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash.egg-info/requires.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)        8 2018-02-15 23:01:27.000000 clkhash-0.9.0/clkhash.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)     2549 2018-02-15 23:00:15.000000 clkhash-0.9.0/README.md
+-rw-r--r--   0 brian     (1000) brian     (1000)       67 2018-02-15 23:01:27.000000 clkhash-0.9.0/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1000)      752 2018-02-15 23:00:15.000000 clkhash-0.9.0/setup.py
+-rw-r--r--   0 brian     (1000) brian     (1000)      253 2018-02-15 23:01:27.000000 clkhash-0.9.0/PKG-INFO
```

### Comparing `clkhash-0.8.1/clkhash/data/CSV_Database_of_Last_Names.csv` & `clkhash-0.9.0/clkhash/data/CSV_Database_of_Last_Names.csv`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/data/female-first-names.csv` & `clkhash-0.9.0/clkhash/data/female-first-names.csv`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/data/first-name-counts-by-year.csv` & `clkhash-0.9.0/clkhash/data/first-name-counts-by-year.csv`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/data/male-first-names.csv` & `clkhash-0.9.0/clkhash/data/male-first-names.csv`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/benchmark.py` & `clkhash-0.9.0/clkhash/benchmark.py`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/bloomfilter.py` & `clkhash-0.9.0/clkhash/bloomfilter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,167 @@
 #!/usr/bin/env python3
 
 """
 Generate a Bloom filter
 """
-from typing import Tuple, Any, Iterable, List
 
 import base64
+from hashlib import sha1, md5
 import hmac
 import sys
 
 from clkhash.identifier_types import IdentifierType
-from hashlib import sha1, md5
 
 from bitarray import bitarray
+from future.builtins import range
+from typing import Tuple, Any, Iterable, List
 
 
 def double_hash_encode_ngrams(ngrams,          # type: Iterable[str]
                               key_sha1,        # type: bytes
                               key_md5,         # type: bytes
                               k,               # type: int
                               l                # type: int
                               ):
-    # type: (...) -> bitarray.bitarray
+    # type: (...) -> bitarray
     """
     computes the double hash encoding of the provided ngrams with the given keys.
 
     Using the method from
     http://www.record-linkage.de/-download=wp-grlc-2011-02.pdf
 
     :param ngrams: list of n-grams to be encoded
     :param key_sha1: hmac secret keys for sha1 as bytes
     :param key_md5: hmac secret keys for md5 as bytes
     :param k: number of hash functions to use per element of the ngrams
     :param l: length of the output bitarray
-    :return bitarray of length l with the bits set which correspond to the encoding of the ngrams
+
+    :return: bitarray of length l with the bits set which correspond to the encoding of the ngrams
     """
     bf = bitarray(l)
     bf.setall(False)
     for m in ngrams:
         sha1hm = int(hmac.new(key_sha1, m.encode(), sha1).hexdigest(), 16) % l
         md5hm = int(hmac.new(key_md5, m.encode(), md5).hexdigest(), 16) % l
         for i in range(k):
             gi = (sha1hm + i * md5hm) % l
             bf[gi] = 1
     return bf
 
 
-def crypto_bloom_filter(record,         # type: Tuple[Any, ...]
-                        tokenizers,     # type: Iterable[IdentifierType]
-                        keys1,          # type: Tuple[bytes, ...]
-                        keys2,          # type: Tuple[bytes, ...]
-                        l=1024,         # type: int
-                        k=30            # type: int
+def fold_xor(bloomfilter,  # type: bitarray
+             folds         # type: int
+             ):
+    # type: (...) -> bitarray
+    """ Performs XOR folding on a Bloom filter.
+
+        If the length of the original Bloom filter is n and we perform
+        r folds, then the length of the resulting filter is n / 2 ** r.
+
+        :param bloomfilter: Bloom filter to fold
+        :param folds: number of folds
+
+        :return: folded bloom filter
+    """
+
+    if len(bloomfilter) % 2 ** folds != 0:
+        msg = ('The length of the bloom filter is {length}. It is not '
+               'divisible by 2 ** {folds}, so it cannot be folded {folds} '
+               'times.'
+               .format(length=len(bloomfilter), folds=folds))
+        raise ValueError(msg)
+
+    for _ in range(folds):
+        bf1 = bloomfilter[:len(bloomfilter) // 2]
+        bf2 = bloomfilter[len(bloomfilter) // 2:]
+
+        bloomfilter = bf1 ^ bf2
+
+    return bloomfilter
+
+
+def crypto_bloom_filter(record,       # type: Tuple[Any, ...]
+                        tokenizers,   # type: Iterable[IdentifierType]
+                        keys1,        # type: Tuple[bytes, ...]
+                        keys2,        # type: Tuple[bytes, ...]
+                        xor_folds=0,  # type: int
+                        l=1024,       # type: int
+                        k=30          # type: int
                         ):
     # type: (...) -> Tuple[bitarray, int, int]
     """
     Makes a Bloom filter from a record with given tokenizers and lists of keys.
 
     Using the method from
     http://www.record-linkage.de/-download=wp-grlc-2011-02.pdf
 
     :param record: plaintext record tuple. E.g. (index, name, dob, gender)
     :param tokenizers: A list of IdentifierType tokenizers (one for each record element)
     :param keys1: list of keys for first hash function as list of bytes
     :param keys2: list of keys for second hash function as list of bytes
+    :param xor_folds: number of XOR folds to perform
     :param l: length of the Bloom filter in number of bits
     :param k: number of hash functions to use per element
 
     :return: 3-tuple:
             - bloom filter for record as a bitarray
             - first element of record (usually an index)
             - number of bits set in the bloomfilter
     """
     bloomfilter = bitarray(l)
     bloomfilter.setall(False)
 
     for (entry, tokenizer, key1, key2) in zip(record, tokenizers, keys1, keys2):
-        ngrams = [ngram for ngram in tokenizer(entry)]
-        bloomfilter |= double_hash_encode_ngrams(ngrams, key1, key2, k, l)
+        ngrams = [ngram for ngram in tokenizer(str(entry))]
+        if tokenizer.weight < 0:
+            raise ValueError('weight must not be smaller than zero, but was: {}'.format(tokenizer.weight))
+        adjusted_k = int(round(tokenizer.weight * k))
+        bloomfilter |= double_hash_encode_ngrams(ngrams, key1, key2, adjusted_k, l)
+
+    bloomfilter = fold_xor(bloomfilter, xor_folds)
 
     return bloomfilter, record[0], bloomfilter.count()
 
 
 def stream_bloom_filters(dataset,       # type: Iterable[Tuple[Any, ...]]
                          schema_types,  # type: Iterable[IdentifierType]
-                         keys           # type: Tuple[Tuple[bytes, ...],Tuple[bytes, ...]]
+                         keys,          # type: Tuple[Tuple[bytes, ...],Tuple[bytes, ...]]
+                         xor_folds=0    # type: int
                          ):
     # type: (...) -> Iterable[Tuple[bitarray, Any, int]]
     """
     Yield bloom filters
 
     :param dataset: An iterable of indexable records.
     :param schema_types: An iterable of identifier type names.
     :param keys: A tuple of two lists of secret keys used in the HMAC.
+    :param xor_folds: number of XOR folds to perform
     :return: Yields bloom filters as 3-tuples
     """
     for s in dataset:
-        yield crypto_bloom_filter(s, schema_types, keys1=keys[0], keys2=keys[1])
+        yield crypto_bloom_filter(s, schema_types, keys[0], keys[1],
+                                  xor_folds=xor_folds)
 
 
-def calculate_bloom_filters(dataset,    # type: Iterable[Tuple[Any]]
-                            schema,     # type: Iterable[IdentifierType]
-                            keys        # type: Tuple[Tuple[bytes], Tuple[bytes]]
+def calculate_bloom_filters(dataset,     # type: Iterable[Tuple[Any]]
+                            schema,      # type: Iterable[IdentifierType]
+                            keys,        # type: Tuple[Tuple[bytes], Tuple[bytes]]
+                            xor_folds=0  # type: int
                             ):
     # type: (...) -> List[Tuple[bitarray, Any, int]]
     """
     :param dataset: A list of indexable records.
     :param schema: An iterable of identifier types.
     :param keys: A tuple of two lists of secret keys used in the HMAC.
+    :param xor_folds: number of XOR folds to perform
     :return: List of bloom filters as 3-tuples, each containing
              bloom filter (bitarray), record first element - usually index, bitcount (int)
     """
-    return list(stream_bloom_filters(dataset, schema, keys))
+    return list(stream_bloom_filters(dataset, schema, keys, xor_folds=xor_folds))
 
 
 def serialize_bitarray(ba):
     # type: (bitarray) -> str
     """Serialize a bitarray (bloomfilter)
 
     """
-
-    # Encode bitarray according to the Python version
-    if sys.version_info[0] >= 3:
-        return base64.encodebytes(ba.tobytes()).decode('utf8')
-    else:
-        return base64.b64encode(ba.tobytes()).decode('utf8')
+    return base64.b64encode(ba.tobytes()).decode('utf8')
```

### Comparing `clkhash-0.8.1/clkhash/cli.py` & `clkhash-0.9.0/clkhash/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 @cli.command('hash', short_help="generate hashes from local PII data")
 @click.argument('input', type=click.File('r'))
 @click.argument('keys', nargs=2, type=click.Tuple([str, str]))
 @click.option('--schema', '-s', type=click.File('r'), default=None)
 @click.argument('output', type=click.File('w'))
 @click.option('-q', '--quiet', default=False, is_flag=True, help="Quiet any progress messaging")
 @click.option('--no-header', default=False, is_flag=True, help="Don't skip the first row")
-def hash(input, output, schema, keys, quiet, no_header):
+@click.option('--xor-folds', default=0, type=click.IntRange(0, None))
+def hash(input, output, schema, keys, quiet, no_header, xor_folds):
     """Process data to create CLKs
 
     Given a file containing csv data as INPUT, and optionally a json
     document defining the expected schema, verify the schema, then
     hash the data to create CLKs writing to OUTPUT. Note the CSV
     file should contain a header row - however this row is not used
     by this tool.
@@ -66,15 +67,15 @@
     $clkutil hash input.txt horse staple output.txt
 
     Use "-" to output to stdout.
     """
 
     schema_types = get_schema_types(load_schema(schema))
 
-    clk_data = clk.generate_clk_from_csv(input, keys, schema_types, no_header, not quiet)
+    clk_data = clk.generate_clk_from_csv(input, keys, schema_types, no_header, not quiet, xor_folds)
     json.dump({'clks': clk_data}, output)
     log("CLK data written to {}".format(output.name))
 
 
 @cli.command('status', short_help='Get status of entity service')
 @click.option('--server', type=str, default=DEFAULT_SERVICE_URL, help="Server address including protocol")
 @click.option('-o','--output', type=click.File('w'), default='-')
```

### Comparing `clkhash-0.8.1/clkhash/clk.py` & `clkhash-0.9.0/clkhash/clk.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,40 +17,45 @@
 from clkhash.bloomfilter import stream_bloom_filters, calculate_bloom_filters, serialize_bitarray
 from clkhash.key_derivation import generate_key_lists
 from clkhash.identifier_types import IdentifierType
 
 log = logging.getLogger('clkhash.clk')
 
 
-def hash_and_serialize_chunk(chunk_pii_data,    # type: Iterable[Tuple[Any]]
-                             schema_types,      # type: Iterable[IdentifierType]
-                             keys               # type: Tuple[Tuple[bytes, ...], Tuple[bytes, ...]]
+def hash_and_serialize_chunk(chunk_pii_data, # type: Iterable[Tuple[Any]]
+                             schema_types,   # type: Iterable[IdentifierType]
+                             keys,           # type: Tuple[Tuple[bytes, ...], Tuple[bytes, ...]]
+                             xor_folds       # type: int
                              ):
     # type: (...) -> List[str]
     """
     Generate Bloom filters (ie hash) from chunks of PII then serialize
     the generated Bloom filters.
 
     :param chunk_pii_data: An iterable of indexable records.
     :param schema_types: An iterable of identifier type names.
     :param keys: A tuple of two lists of secret keys used in the HMAC.
+    :param xor_folds: Number of XOR folds to perform. Each fold halves
+        the hash length.
     :return: A list of serialized Bloom filters
     """
     clk_data = []
-    for clk in stream_bloom_filters(chunk_pii_data, schema_types, keys):
+    for clk in stream_bloom_filters(chunk_pii_data, schema_types,
+                                    keys, xor_folds):
         clk_data.append(serialize_bitarray(clk[0]).strip())
 
     return clk_data
 
 
-def generate_clk_from_csv(input,            # type: TextIO
-                          keys,             # type: Tuple[Union[bytes, str], Union[bytes, str]]
-                          schema_types,     # type: List[IdentifierType]
-                          no_header=False,  # type: bool
-                          progress_bar=True # type: bool
+def generate_clk_from_csv(input,             # type: TextIO
+                          keys,              # type: Tuple[Union[bytes, str], Union[bytes, str]]
+                          schema_types,      # type: List[IdentifierType]
+                          no_header=False,   # type: bool
+                          progress_bar=True, # type: bool
+                          xor_folds=0        # type: int
                           ):
     # type: (...) -> List[str]
     log.info("Hashing data")
 
     # Read from CSV file
     reader = csv.reader(input)
 
@@ -68,25 +73,27 @@
 
     # generate two keys for each identifier
     key_lists = generate_key_lists(keys, len(schema_types))
 
     if progress_bar:
         with tqdm(desc="generating CLKs", total=len(pii_data), unit='clk', unit_scale=True) as pbar:
             progress_bar_callback = lambda update: pbar.update(update)
-            results = generate_clks(pii_data, schema_types, key_lists, progress_bar_callback)
+            results = generate_clks(pii_data, schema_types, key_lists,
+                                    xor_folds, progress_bar_callback)
     else:
-        results = generate_clks(pii_data, schema_types, key_lists)
+        results = generate_clks(pii_data, schema_types, key_lists, xor_folds)
 
     log.info("Hashing took {:.2f} seconds".format(time.time() - start_time))
     return results
 
 
 def generate_clks(pii_data,         # type: Sequence[Tuple[str, ...]]
                   schema_types,     # type: List[IdentifierType]
                   key_lists,        # type: Tuple[Tuple[bytes, ...], ...]
+                  xor_folds,        # type: int
                   callback=None     # type: Optional[Callable[[int], None]]
                   ):
     # type: (...) -> List[Any]
     results = []
 
     # Chunks PII
     log.info("Hashing {} entities".format(len(pii_data)))
@@ -94,27 +101,29 @@
 
     # If running Python3 parallelise hashing.
     if sys.version_info[0] >= 3:
         # Compute Bloom filter from the chunks and then serialise it
         with concurrent.futures.ProcessPoolExecutor() as executor:
             futures = []
             for chunk in chunks(pii_data, chunk_size):
-                future = executor.submit(hash_and_serialize_chunk,
-                                         chunk, schema_types, key_lists)
+                future = executor.submit(
+                    hash_and_serialize_chunk,
+                    chunk, schema_types, key_lists, xor_folds)
                 if callback is not None:
                     future.add_done_callback(lambda f: callback(len(f.result())))
                 futures.append(future)
 
             for future in futures:
                 results.extend(future.result())
 
     else:
         log.info("Hashing with one core, upgrade to python 3 to utilise all cores")
         for chunk in chunks(pii_data, chunk_size):
-            results.extend(hash_and_serialize_chunk(chunk, schema_types, key_lists))
+            results.extend(hash_and_serialize_chunk(chunk, schema_types,
+                                                    key_lists, xor_folds))
             if callback is not None:
                 callback(len(chunk))
     return results
 
 T = TypeVar('T')      # Declare generic type variable
```

### Comparing `clkhash-0.8.1/clkhash/identifier_types.py` & `clkhash-0.9.0/clkhash/identifier_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 """
 Convert PII to tokens
 """
-from typing import Dict, List, NoReturn, Any, Callable, Union, Optional
+from typing import Dict, List, Any
 
 from clkhash.tokenizer import unigramlist, bigramlist
+from copy import copy
 
 
 class IdentifierType:
     """
     Base class used for all identifier types.
 
     Required to provide a mapping of schema to hash type
     uni-gram or bi-gram.
     """
 
     def __init__(self, unigram=False, weight=1, **kwargs):
-        # type: (bool, int, Any) -> None
+        # type: (bool, float, Any) -> None
         """
-        :param unigram: Use uni-gram instead of using bi-grams
-        :param int weight: How many times to include this identifier.
+        :param bool unigram: Use uni-gram instead of using bi-grams
+        :param float weight: adjusts the "importance" of this identifier in the Bloom filter. Can be set to zero to skip
         :param kwargs: Extra keyword arguments passed to the tokenizer
-        Can be set to zero to skip
+
+        .. Note::
+           For each n-gram of an identifier, we compute *k* different indices in the Bloom filter which will be set to
+           true. There is a global :math:`k_{default}` value, and the *k* value for each identifier is computed as
+
+           .. math::
+              k = weight * k_{default},
+
+           rounded to the nearest integer.
+
+           Reasons why you might want to set weights:
+
+             - Long identifiers like street name will produce a lot more n-grams than small identifiers like zip code.
+               Thus street name will flip more bits in the Bloom filter and will have a bigger influence in the overall
+               matching score.
+
+             - The matching might produce better results if identifiers that are stable and / or have low error rates
+               are given higher prominence in the Bloom filter.
+
         """
-        self.weight = int(weight)
+        self.weight = weight
         self.tokenizer = unigramlist if unigram else bigramlist
         self.kwargs = kwargs
 
     def __call__(self, entry):
         # type: (str) -> List[str]
-        result = []
-        for i in range(self.weight):
-            for token in self.tokenizer(entry, **self.kwargs):      # type: ignore
-                result.append(token)
+        return self.tokenizer(entry, **self.kwargs)  # type: ignore
 
-        return result
 
 basic_types = {
     'INDEX': IdentifierType(weight=0),
 
     'GENDER M or F': IdentifierType(unigram=True),
     'GENDER freetext': IdentifierType(),
 
@@ -97,10 +112,11 @@
     else:
         id_type = IdentifierType(
             weight=schema_object.get('weight', 1)
         )
 
     # check if there was a custom weight
     if 'weight' in schema_object:
+        id_type = copy(id_type)  # we don't want to modify the original
         id_type.weight = schema_object['weight']
 
     return id_type
```

### Comparing `clkhash-0.8.1/clkhash/key_derivation.py` & `clkhash-0.9.0/clkhash/key_derivation.py`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/randomnames.py` & `clkhash-0.9.0/clkhash/randomnames.py`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/schema.py` & `clkhash-0.9.0/clkhash/schema.py`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash/tokenizer.py` & `clkhash-0.9.0/clkhash/tokenizer.py`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/clkhash.egg-info/SOURCES.txt` & `clkhash-0.9.0/clkhash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clkhash-0.8.1/README.md` & `clkhash-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # CLK Hash
 
 Python implementation of cryptographic linkage key hashing. Supports Python versions 2.7+, 3.4+
 
 This is as described by Rainer Schnell, Tobias Bachteler, and Jörg Reiher in
 [A Novel Error-Tolerant Anonymous Linking Code](http://www.record-linkage.de/-download=wp-grlc-2011-02.pdf)
 
+[![Documentation Status](https://readthedocs.org/projects/clkhash/badge/?version=latest)](http://clkhash.readthedocs.io/en/latest/?badge=latest)
+
 
 # Installation
 
 Install the dependencies with:
 
     pip install -r requirements.txt
```

### Comparing `clkhash-0.8.1/setup.py` & `clkhash-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import setup, find_packages
 
 requirements = [
         "bitarray==0.8.1",
         "click==6.7",
-        "requests==2.18.1",
+        "requests==2.18.4",
         "futures==3.1.1",
         "cryptography==2.1.3",
         "tqdm==4.19.4",
-        "typing"
+        "typing",
+        "future==0.16.0",
+        "typing>=3.6.2"
     ]
 
 setup(
     name="clkhash",
-    version='0.8.1',
+    version='0.9.0',
     description='Hash utility to create Cryptographic Linkage Keys',
     url='https://github.com/n1analytics/clkhash',
     license='Apache',
     install_requires=requirements,
     test_requires=['nose>=1.3'],
     packages=find_packages(exclude=['tests']),
     package_data={'clkhash': ['data/*.csv']},
```

