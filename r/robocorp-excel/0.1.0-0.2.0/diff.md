# Comparing `tmp/robocorp_excel-0.1.0.tar.gz` & `tmp/robocorp_excel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_excel-0.1.0.tar", max compression
+gzip compressed data, was "robocorp_excel-0.2.0.tar", max compression
```

## Comparing `robocorp_excel-0.1.0.tar` & `robocorp_excel-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0       25 2023-04-04 11:49:45.059148 robocorp_excel-0.1.0/README.md
--rw-r--r--   0        0        0      609 2023-04-04 11:49:45.059710 robocorp_excel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       76 2023-04-04 11:49:45.059983 robocorp_excel-0.1.0/src/robo/libs/excel/__init__.py
--rw-r--r--   0        0        0      598 2023-04-04 11:49:45.060207 robocorp_excel-0.1.0/src/robo/libs/excel/_types.py
--rw-r--r--   0        0        0    22691 2023-04-04 11:49:45.060522 robocorp_excel-0.1.0/src/robo/libs/excel/_workbooks.py
--rw-r--r--   0        0        0     3993 2023-04-04 11:49:45.060775 robocorp_excel-0.1.0/src/robo/libs/excel/_worksheet.py
--rw-r--r--   0        0        0     1297 2023-04-04 11:49:45.061011 robocorp_excel-0.1.0/src/robo/libs/excel/excel.py
--rw-r--r--   0        0        0    64921 2023-04-04 11:49:45.061605 robocorp_excel-0.1.0/src/robo/libs/excel/tables.py
--rw-r--r--   0        0        0       60 2023-04-04 11:49:45.061857 robocorp_excel-0.1.0/src/robo/libs/excel/types.py
--rw-r--r--   0        0        0     2460 2023-04-04 11:49:45.062008 robocorp_excel-0.1.0/src/robo/libs/excel/workbook.py
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 robocorp_excel-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-04-04 11:49:45.059148 robocorp_excel-0.2.0/README.md
+-rw-r--r--   0        0        0      615 2023-04-25 10:40:48.282657 robocorp_excel-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-04-25 10:39:03.644567 robocorp_excel-0.2.0/src/robocorp/excel/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-25 10:39:03.644677 robocorp_excel-0.2.0/src/robocorp/excel/_types.py
+-rw-r--r--   0        0        0    23104 2023-04-25 10:39:03.645036 robocorp_excel-0.2.0/src/robocorp/excel/_workbooks.py
+-rw-r--r--   0        0        0     2639 2023-04-25 10:39:03.645269 robocorp_excel-0.2.0/src/robocorp/excel/excel.py
+-rw-r--r--   0        0        0    65743 2023-04-25 10:39:03.645757 robocorp_excel-0.2.0/src/robocorp/excel/tables.py
+-rw-r--r--   0        0        0     2854 2023-04-25 10:39:03.645940 robocorp_excel-0.2.0/src/robocorp/excel/workbook.py
+-rw-r--r--   0        0        0     5425 2023-04-25 10:39:03.646107 robocorp_excel-0.2.0/src/robocorp/excel/worksheet.py
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 robocorp_excel-0.2.0/PKG-INFO
```

### Comparing `robocorp_excel-0.1.0/pyproject.toml` & `robocorp_excel-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "robocorp-excel"
-version = "0.1.0"
+version = "0.2.0"
 description = "Robocorp Excel automation library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
     "Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
-packages = [{include = "robo", from="src"}]
+packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
+pillow = "^9.1.1"
 xlrd = "^2.0.1"
 xlwt = "^1.3.0"
 xlutils = "^2.0.0"
 openpyxl = "^3.0.9"
 
 [tool.poetry.group.dev.dependencies]
-libs-devdeps = {path = "..", develop = true}
+libs-devdeps = {path = ".."}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_excel-0.1.0/src/robo/libs/excel/_types.py` & `robocorp_excel-0.2.0/src/robocorp/excel/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.1.0/src/robo/libs/excel/_workbooks.py` & `robocorp_excel-0.2.0/src/robocorp/excel/_workbooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,37 @@
 import xlwt
 
 from xlutils.copy import copy as xlutils_copy
 from openpyxl.worksheet.cell_range import CellRange
 from openpyxl.utils import get_column_letter
 from openpyxl.utils.exceptions import InvalidFileException
 
-from robo.libs.excel._types import PathType
-from robo.libs.excel.tables import Table
-from robo.libs.excel._worksheet import Worksheet
+from robocorp.excel._types import PathType
+from robocorp.excel.tables import Table
+from robocorp.excel.worksheet import Worksheet
 
 
 def _get_column_index(column: str) -> int:
     """Get column index from name, e.g. A -> 1, D -> 4, AC -> 29.
+
     Reverse of `get_column_letter()`
     """
     column = str(column).lower()
 
     col = 0
     for digit, char in enumerate(column[::-1]):
         value = ord(char) - 96
         col += (26**digit) * value
 
     return col
 
 
 def _ensure_unique(values: Any) -> List[Any]:
     """Ensures that each string value in the list is unique.
+
     Adds a suffix to each value that has duplicates,
     e.g. [Banana, Apple, Lemon, Apple] -> [Banana, Apple, Lemon, Apple_2]
     """
 
     def to_unique(values: Any) -> List[Any]:
         output = []
         seen = defaultdict(int)
@@ -90,42 +92,45 @@
     raise ValueError(
         f'Failed to open Excel file ("{path}"), '
         "verify that the path and extension are correct"
     )
 
 
 class BaseWorkbook:
-
     """Common logic for both .xls and .xlsx files management."""
 
     def __init__(self, path: Optional[PathType] = None):
         self.logger = logging.getLogger(__name__)
         # TODO: type hint these
+        self.path = path
         self._book = None
         self._extension = None
         self._active = None
 
     @property
     def book(self):
         return self._book
 
+    def open(self, path, read_only=False, write_only=False, data_only=False):
+        self.path = path
+
     def worksheet(self, name: str) -> Worksheet:
         return Worksheet(self, name)
 
     def _validate_content(self, props_obj: Any):
         # Strips leading/trailing whitespace in Excel properties.
         public_props = [prop for prop in dir(props_obj) if not prop.startswith("_")]
         for prop in public_props:
             value = getattr(props_obj, prop)
             if value and isinstance(value, str):
                 setattr(props_obj, prop, value.strip())
 
 
 class XlsxWorkbook(BaseWorkbook):
-    """Container for manipulating modern Excel files (.xlsx)"""
+    """Container for manipulating modern Excel files (.xlsx)."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._read_only = False
 
     @staticmethod
     def is_sheet_empty(sheet):
@@ -219,26 +224,31 @@
             options["write_only"] = True
 
         if extension in (".xlsm", ".xltm"):
             options["keep_vba"] = True
 
         self._book = openpyxl.load_workbook(**options)
         self._extension = extension
+        super().open(path, read_only, write_only, data_only)
 
     def close(self):
         self._book.close()
         self._book = None
         self._extension = None
         self._active = None
 
     def validate_content(self):
         self._validate_content(self._book.properties)
 
-    def save(self, path: PathType):
-        path = str(pathlib.Path(path))
+    def save(self, path: Union[PathType, BytesIO]):
+        if not isinstance(path, BytesIO):
+            path = str(pathlib.Path(path))
+        if not path:
+            raise ValueError("No path defined for workbook")
+
         self._book.save(filename=path)
 
     def create_worksheet(self, name):
         self._book.create_sheet(title=name)
         self.active = name
 
     def read_worksheet(self, name=None, header=False, start=None) -> List[dict]:
@@ -398,15 +408,15 @@
 
         img = openpyxl.drawing.image.Image(image)
         img.anchor = cell
         sheet.add_image(img)
 
 
 class XlsWorkbook(BaseWorkbook):
-    """Container for manipulating legacy Excel files (.xls)"""
+    """Container for manipulating legacy Excel files (.xls)."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._images = []
 
     @staticmethod
     def is_sheet_empty(sheet):
@@ -439,15 +449,15 @@
             match = int(sheet.name == value)
             sheet.sheet_selected = match
             sheet.sheet_visible = match
 
         self._active = value
 
     @property
-    def extension(self):
+    def extension(self) -> Optional[str]:
         return self._extension
 
     def _get_sheetname(self, name):
         if self._book.nsheets == 0:
             raise ValueError("No worksheets in file")
 
         if name is None:
@@ -535,16 +545,17 @@
             self.open(fd)
         finally:
             fd.close()
 
     def validate_content(self):
         self._validate_content(self._book)
 
-    def save(self, path: PathType):
-        path = str(pathlib.Path(path))
+    def save(self, path: Union[PathType, BytesIO]):
+        if not isinstance(path, BytesIO):
+            path = str(pathlib.Path(path))
         if not path:
             raise ValueError("No path defined for workbook")
 
         book = xlutils_copy(self._book)
         self._insert_images(book)
         book.save(path)
```

### Comparing `robocorp_excel-0.1.0/src/robo/libs/excel/tables.py` & `robocorp_excel-0.2.0/src/robocorp/excel/tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     List,
     NamedTuple,
     Optional,
     Tuple,
     Union,
 )
 
-from robo.libs.excel._types import is_dict_like, is_list_like, is_namedtuple
+from robocorp.excel._types import is_dict_like, is_list_like, is_namedtuple
 
 
 Index = Union[int, str]
 Column = Union[int, str]
 Row = Union[Dict, List, Tuple, NamedTuple, set]
 Data = Optional[Union[Dict[Column, Row], List[Row], "Table"]]
 CellCondition = Callable[[Any], bool]
@@ -49,15 +49,15 @@
     if not is_list_like(obj):
         return [obj] * int(size)
     else:
         return obj
 
 
 def to_identifier(val: Any):
-    """Convert string to valid identifier"""
+    """Convert string to valid identifier."""
     val = str(val).strip()
     # Replaces spaces, dashes, and slashes to underscores
     val = re.sub(r"[\s\-/\\]", "_", val)
     # Remove remaining invalid characters
     val = re.sub(r"[^0-9a-zA-Z_]", "", val)
     # Identifier can't start with digits
     val = re.sub(r"^[^a-zA-Z_]+", "", val)
@@ -95,50 +95,56 @@
 def if_none(value: Any, default: Any):
     """Return default if value is None."""
     return value if value is not None else default
 
 
 def uniq(seq: Iterable):
     """Return list of unique values while preserving order.
+
     Values must be hashable.
     """
     seen, result = {}, []
     for item in seq:
         if item in seen:
             continue
         seen[item] = None
         result.append(item)
     return result
 
 
 class Dialect(Enum):
-    """CSV dialect"""
+    """CSV dialect."""
 
     Excel = "excel"
     ExcelTab = "excel-tab"
     Unix = "unix"
 
 
 class Table:
     """Container class for tabular data.
 
-    Supported data formats:
+    Note:
+        Supported data formats:
 
-    - empty: None values populated according to columns/index
-    - list: list of data Rows
-    - dict: Dictionary of columns as keys and Rows as values
-    - table: An existing Table
+        - empty: None values populated according to columns/index
+        - list: list of data Rows
+        - dict: Dictionary of columns as keys and Rows as values
+        - table: An existing Table
 
-    Row: a namedtuple, dictionary, list or a tuple
+        Row: a namedtuple, dictionary, list or a tuple
 
-    :param data:     Values for table,  see "Supported data formats"
-    :param columns:  Names for columns, should match data dimensions
     """
 
     def __init__(self, data: Data = None, columns: Optional[List[str]] = None):
+        """Creates a Table object.
+
+        Args:
+            data:     Values for table,  see ``Supported data formats``
+            columns:  Names for columns, should match data dimensions
+        """
         self._data = []
         self._columns = []
 
         # Use public setter to validate data
         if columns is not None:
             self.columns = list(columns)
 
@@ -481,16 +487,18 @@
 
         If either `indexes` or `columns` is a list:
             Returns matching row or column
 
         If both `indexes` and `columns` are lists:
             Returns a new Table instance with matching cell values
 
-        :param indexes: List of indexes, or all if not given
-        :param columns: List of columns, or all if not given
+        Args:
+            indexes: List of indexes, or all if not given.
+            columns: List of columns, or all if not given.
+            as_list: Return as list, instead of dictionary.
         """
         indexes = if_none(indexes, self.index)
         columns = if_none(columns, self._columns)
 
         if is_list_like(indexes) and is_list_like(columns):
             return self.get_table(indexes, columns, as_list)
         elif not is_list_like(indexes) and is_list_like(columns):
@@ -506,17 +514,18 @@
         col = self.column_location(column)
 
         return self._data[idx][col]
 
     def get_row(self, index: Index, columns=None, as_list=False):
         """Get column values from row.
 
-        :param index:   Index for row
-        :param columns: Column names to include, or all if not given
-        :param as_list: Return row as dictionary, instead of list
+        Args:
+            index:   Index for row.
+            columns: Column names to include, or all if not given.
+            as_list: Return row as list, instead of dictionary.
         """
         columns = if_none(columns, self._columns)
         idx = self.index_location(index)
 
         if as_list:
             row = []
             for column in columns:
@@ -529,17 +538,18 @@
                 col = self.column_location(column)
                 row[self._columns[col]] = self._data[idx][col]
             return row
 
     def get_column(self, column, indexes=None, as_list=False):
         """Get row values from column.
 
-        :param column: Name for column
-        :param indexes: Row indexes to include, or all if not given
-        :param as_list: Return column as dictionary, instead of list
+        Args:
+            column: Name for column
+            indexes: Row indexes to include, or all if not given
+            as_list: Return column as dictionary, instead of list
         """
         indexes = if_none(indexes, self.index)
         col = self.column_location(column)
 
         if as_list:
             column = []
             for index in indexes:
@@ -549,15 +559,17 @@
         else:
             column = {}
             for index in indexes:
                 idx = self.index_location(index)
                 column[idx] = self._data[idx][col]
             return column
 
-    def get_table(self, indexes=None, columns=None, as_list=False):
+    def get_table(
+        self, indexes=None, columns=None, as_list=False
+    ) -> Union[List, "Table"]:
         """Get a new table from all cells matching indexes and columns."""
         indexes = if_none(indexes, self.index)
         columns = if_none(columns, self._columns)
 
         if indexes == self.index and columns == self._columns:
             return self.copy()
 
@@ -609,19 +621,19 @@
             row.append(None)
 
         return len(self._columns) - 1
 
     def set(self, indexes=None, columns=None, values=None):
         """Sets multiple cell values at a time.
 
-        Both `indexes` and `columns` can be scalar or list-like,
+        Both ``indexes`` and ``columns`` can be scalar or list-like,
         which enables setting individual cells, rows/columns, or regions.
 
-        If `values` is scalar, all matching cells will be set to that value.
-        Otherwise the length should match the cell count defined by the
+        If ``values`` is scalar, all matching cells will be set to that value.
+        Otherwise, the length should match the cell count defined by the
         other parameters.
         """
         indexes = to_list(if_none(indexes, self.index))
         columns = to_list(if_none(columns, self._columns))
 
         size = len(indexes) + len(columns)
         values = to_list(values, size=size)
@@ -632,14 +644,15 @@
             idx = self.index_location(index)
             for column in columns:
                 col = self.column_location(column)
                 self.set_cell(index, column, values[idx + col])
 
     def set_cell(self, index, column, value):
         """Set individual cell value.
+
         If either index or column is missing, they are created.
         """
         try:
             idx = self.index_location(index)
         except (IndexError, ValueError):
             idx = self._add_row(index)
 
@@ -738,18 +751,21 @@
         # Create sort criteria list, with each row as tuple of column values
         values = (self.get_column(column, as_list=True) for column in columns)
         values = list(zip(*values))
         assert len(values) == self.size
 
         def sorter(row):
             """Sort table by given values, while allowing for disparate types.
-            Order priority:
+
+            Note:
+                Order priority:
                 - Values by typename
                 - Numeric types
                 - None values
+
             """
             criteria = []
             for value in row[1]:  # Ignore enumeration
                 criteria.append(
                     (
                         value is not None,
                         "" if isinstance(value, Number) else type(value).__name__,
@@ -827,14 +843,15 @@
             row = {"index": index} if with_index else {}
             for column in self._columns:
                 row[column] = self.get_cell(index, column)
             yield row
 
     def iter_tuples(self, with_index=True, name="Row"):
         """Iterate rows with values as namedtuples.
+
         Converts column names to valid Python identifiers,
         e.g. "First Name" -> "First_Name"
         """
         columns = {column: to_identifier(column) for column in self._columns}
 
         fields = ["index"] if with_index else []
         fields.extend(columns.values())
@@ -873,15 +890,15 @@
                 value = self.get_cell(index, column)
                 export[column].append(value)
 
         return export
 
 
 class Tables:
-    """`Tables` is a library for manipulating tabular data inside Robot Framework.
+    """``Tables`` is a library for manipulating tabular data.
 
     It can import data from various sources and apply different operations to it.
     Common use-cases are reading and writing CSV files, inspecting files in
     directories, or running tasks using existing Excel data.
 
     **Import types**
 
@@ -932,98 +949,78 @@
     index also starts from zero. Keywords where rows are indexed also support
     negative values, which start counting backwards from the end.
 
     For instance, in a table with five rows, the first row could be referred
     to with the number 0. The last row could be accessed with either 4 or
     -1.
 
-    **Examples**
-
-    **Robot Framework**
-
-    The `Tables` library can load tabular data from various other libraries
-    and manipulate it inside Robot Framework.
-
-    .. code-block:: robotframework
+    Examples:
+        The ``Tables`` library can load tabular data from various other libraries
+        and manipulate it.
 
-        *** Settings ***
-        Library    RPA.Tables
+        .. code-block:: python
 
-        *** Keywords ***
-        Files to Table
-            ${files}=    List files in directory    ${CURDIR}
-            ${files}=    Create table    ${files}
-            Filter table by column    ${files}    size  >=  ${1024}
-            FOR    ${file}    IN    @{files}
-                Log    ${file}[name]
-            END
-            Write table to CSV    ${files}    ${OUTPUT_DIR}${/}files.csv
+            from robocorp.excel.tables import Tables
 
-    **Python**
-
-    The library is also available directly through Python, where it
-    is easier to handle multiple different tables or do more bespoke
-    manipulation operations.
-
-    .. code-block:: python
+            tables = Tables()
+            orders = tables.read_table_from_csv(
+                "orders.csv", columns=["name", "mail", "product"]
+            )
 
-        from RPA.Tables import Tables
+            customers = tables.group_table_by_column(rows, "mail")
+            for customer in customers:
+                for order in customer:
+                    add_cart(order)
+                make_order()
 
-        library = Tables()
-        orders = library.read_table_from_csv(
-            "orders.csv", columns=["name", "mail", "product"]
-        )
-
-        customers = library.group_table_by_column(rows, "mail")
-        for customer in customers:
-            for order in customer:
-                add_cart(order)
-            make_order()
     """
 
-    ROBOT_LIBRARY_SCOPE = "GLOBAL"
-    ROBOT_LIBRARY_DOC_FORMAT = "REST"
-
     def __init__(self):
         self.logger = logging.getLogger(__name__)
 
     @staticmethod
     def _requires_table(obj: Any):
         if not isinstance(obj, Table):
-            raise TypeError("Keyword requires Table object")
+            raise TypeError("Method requires Table object")
 
     def create_table(
         self, data: Data = None, trim: bool = False, columns: List[str] = None
     ) -> Table:
         """Create Table object from data.
 
         Data can be a combination of various iterable containers, e.g.
         list of lists, list of dicts, dict of lists.
 
-        :param data:    Source data for table
-        :param trim:    Remove all empty rows from the end of the worksheet,
-                        default `False`
-        :param columns: Names of columns (optional)
-        :return:        Table object
+        Args:
+            data:    Source data for table
+            trim:    Remove all empty rows from the end of the worksheet,
+                            default `False`
+            columns: Names of columns (optional)
 
-        See the main library documentation for more information about
+        Returns:
+            Table:  Table object
+
+        See the main documentation for more information about
         supported data types.
 
         Example:
+            .. code-block:: python
+
+                # Create a new table using a Dictionary of Lists
+                # Because of the dictionary keys the column names will be automatically set
+                from robocorp.excel.tables import Tables
+
+                tables = Tables()
+
+                table_data_name = ["Mark", "John", "Amy"]
+                table_data_age = [58, 22, 67]
+                table_data = { name: table_data_name, age: table_data_age }
+                table = tables.create_table(table_data)
 
-        .. code-block:: robotframework
 
-            # Create a new table using a Dictionary of Lists
-            # Because of the dictionary keys the column names will be automatically set
-            @{Table_Data_name}=    Create List    Mark    John    Amy
-            @{Table_Data_age}=    Create List    ${58}    ${22}    ${67}
-            &{Table_Data}=    Create Dictionary
-            ...    name=${Table_Data_name}
-            ...    age=${Table_Data_age}
-            ${table}=    Create Table    ${Table_Data}
         """
         table = Table(data, columns)
 
         if trim:
             self.trim_empty_rows(table)
             self.trim_column_names(table)
 
@@ -1032,102 +1029,119 @@
         return table
 
     def export_table(
         self, table: Table, with_index: bool = False, as_list: bool = True
     ) -> Union[List, Dict]:
         """Convert a table object into standard Python containers.
 
-        :param table:       Table to convert to dict
-        :param with_index:  Include index in values
-        :param as_list:     Export data as list instead of dict
-        :return:            A List or Dictionary that represents the table
+        Args:
+            table:       Table to convert to dict
+            with_index:  Include index in values
+            as_list:     Export data as list instead of dict
+
+        Returns
+            (Union[list, dict]): A List or Dictionary that represents the table
 
         Example:
+        .. code-block:: python
 
-        .. code-block:: robotframework
+            from robocorp.excel.tables import Tables
+
+            tables = Tables()
+
+            table_data_name = ["Mark", "John", "Amy"]
+            table_data_age = [58, 22, 67]
+            table_data = { name: table_data_name, age: table_data_age }
+            table = tables.create_table(table_data)
+
+            # manipulate the table..
+
+            export = tables.export_table(table)
 
-            ${orders}=       Read worksheet as table    orders.xlsx
-            Sort table by column    ${orders}    CustomerId
-            ${export}=       Export table    ${orders}
-            # The following keyword expects a dictionary:
-            Write as JSON    ${export}
         """
         self._requires_table(table)
         if as_list:
             return table.to_list(with_index)
         else:
             return table.to_dict(with_index)
 
     def copy_table(self, table: Table) -> Table:
         """Make a copy of a table object.
 
-        :param table:   Table to copy
-        :return:        Table object
+        Args:
+            table:  Table to copy
+
+        Returns:
+            Table:  Table object
 
-        ${table_copy}=    Copy table    ${table}
         """
         self._requires_table(table)
         return table.copy()
 
     def clear_table(self, table: Table):
         """Clear table in-place, but keep columns.
 
-        :param table:   Table to clear
+        Args:
+            table:   Table to clear
 
         Example:
+        .. code-block:: python
+            from robocorp.excel.tables import Tables
 
-        .. code-block:: robotframework
+            tables = Tables()
+            tables.clear_table(table)
 
-            Clear table    ${table}
         """
         self._requires_table(table)
         table.clear()
 
     def merge_tables(self, *tables: Table, index: Optional[str] = None) -> Table:
         """Create a union of two tables and their contents.
 
-        :param tables: Tables to merge
-        :param index:  Column name to use as index for merge
-        :return:       Table object
+        Args:
+            tables: Tables to merge
+            index:  Column name to use as index for merge
+
+        Returns:
+            Table: Table object
 
-        By default rows from all tables are appended one after the other.
+        By default, rows from all tables are appended one after the other.
         Optionally a column name can be given with ``index``, which is
         used to merge rows together.
 
         Example:
+            For instance, a ``name`` column could be used to identify
+            unique rows and the merge operation should overwrite values
+            instead of appending multiple copies of the same name.
+
+            ====== =====
+            Name   Price
+            ====== =====
+            Egg    10.0
+            Cheese 15.0
+            Ham    20.0
+            ====== =====
+
+            ====== =====
+            Name   Stock
+            ====== =====
+            Egg    12.0
+            Cheese 99.0
+            Ham    0.0
+            ====== =====
+
+        .. code-block:: python
+            from robocorp.excel.tables import Tables
+
+            tables = Tables()
+
+            products = tables.merge_tables(prices, stock, index="Name")
+            for product in products:
+                print(f'Product: {product["Name"]}, Product: {product["Price"]}'
 
-        For instance, a ``name`` column could be used to identify
-        unique rows and the merge operation should overwrite values
-        instead of appending multiple copies of the same name.
-
-        ====== =====
-        Name   Price
-        ====== =====
-        Egg    10.0
-        Cheese 15.0
-        Ham    20.0
-        ====== =====
-
-        ====== =====
-        Name   Stock
-        ====== =====
-        Egg    12.0
-        Cheese 99.0
-        Ham    0.0
-        ====== =====
-
-        .. code-block:: robotframework
-
-            ${products}=    Merge tables    ${prices}    ${stock}    index=Name
-            FOR    ${product}    IN    @{products}
-                Log many
-                ...    Product: ${product}[Name]
-                ...    Price: ${product}[Price]
-                ...    Stock: ${product}[Stock]
-            END
         """
         if index is None:
             return self._merge_by_append(tables)
         else:
             return self._merge_by_index(tables, index)
 
     def _merge_by_append(self, tables: Tuple[Table, ...]):
@@ -1168,43 +1182,46 @@
                         merged.set_cell(row_index, column, value)
 
         return merged
 
     def get_table_dimensions(self, table: Table) -> Tuple[int, int]:
         """Return table dimensions, as (rows, columns).
 
-        :param table:    Table to inspect
-        :return:         Two integer values that represent the number
-                         of rows and columns
+        Args:
+            table:    Table to inspect
+
+        Returns:
+            (Tuple[int, int]): Two integer values that represent the number of rows and columns
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                ${rows}  ${columns}=    Get table dimensions    ${table}
+                Log    Table has ${rows} rows and ${columns} columns.
 
-            ${rows}  ${columns}=    Get table dimensions    ${table}
-            Log    Table has ${rows} rows and ${columns} columns.
         """
         self._requires_table(table)
         return table.dimensions
 
     def rename_table_columns(
         self, table: Table, names: List[Union[str, None]], strict: bool = False
     ):
-        """Renames columns in the Table with given values. Columns with
-        name as ``None`` will use the previous value.
+        """Renames columns in the Table with given values.
 
-        :param table:   Table to modify
-        :param names:   List of new column names
-        :param strict:  If True, raises ValueError if column lengths
+        Columns with name as ``None`` will use the previous value.
+
+        Args:
+            table:   Table to modify
+            names:   List of new column names
+            strict:  If True, raises ValueError if column lengths
                         do not match
 
         The renaming will be done in-place.
 
         Examples:
-
         .. code-block:: robotframework
 
             # Initially set the column names
             ${columns}=    Create list   First  Second  Third
             Rename table columns    ${table}    ${columns}
             # First, Second, Third
 
@@ -1231,371 +1248,405 @@
         table.columns = after
 
     def add_table_column(
         self, table: Table, name: Optional[str] = None, values: Any = None
     ):
         """Append a column to a table.
 
-        :param table:   Table to modify
-        :param name:    Name of new column
-        :param values:  Value(s) for new column
+        Args:
+            table:   Table to modify
+            name:    Name of new column
+            values:  Value(s) for new column
 
         The ``values`` can either be a list of values, one for each row, or
         one single value that is set for all rows.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Add empty column
+                Add table column    ${table}
 
-            # Add empty column
-            Add table column    ${table}
+                # Add empty column with name
+                Add table column    ${table}    name=Home Address
 
-            # Add empty column with name
-            Add table column    ${table}    name=Home Address
+                # Add new column where every every row has the same value
+                Add table column    ${table}    name=TOS    values=${FALSE}
 
-            # Add new column where every every row has the same value
-            Add table column    ${table}    name=TOS    values=${FALSE}
+                # Add new column where every row has a unique value
+                ${is_first}=    Create list    ${TRUE}    ${FALSE}    ${FALSE}
+                Add table column    ${table}    name=IsFirst    values=${is_first}
 
-            # Add new column where every row has a unique value
-            ${is_first}=    Create list    ${TRUE}    ${FALSE}    ${FALSE}
-            Add table column    ${table}    name=IsFirst    values=${is_first}
         """
         self._requires_table(table)
         table.append_column(name, values)
 
     def add_table_row(self, table: Table, values: Any = None):
         """Append rows to a table.
 
-        :param table:   Table to modify
-        :param values:  Value(s) for new row
+        Args:
+            table:   Table to modify
+            values:  Value(s) for new row
 
         The ``values`` can either be a list of values, or a dictionary
         where the keys match current column names. Values for unknown
         keys are discarded.
 
         It can also be a single value that is set for all columns,
         which is ``None`` by default.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Add empty row
+                Add table row    ${table}
 
-            # Add empty row
-            Add table row    ${table}
+                # Add row where every column has the same value
+                Add table row    ${table}    Unknown
 
-            # Add row where every column has the same value
-            Add table row    ${table}    Unknown
+                # Add values per column
+                ${values}=    Create dictionary    Username=Mark    Mail=mark@robocorp.com
+                Add table row    ${table}    ${values}
 
-            # Add values per column
-            ${values}=    Create dictionary    Username=Mark    Mail=mark@robocorp.com
-            Add table row    ${table}    ${values}
         """
         self._requires_table(table)
         table.append_row(values)
 
     def get_table_row(
         self, table: Table, row: Index, as_list: bool = False
     ) -> Union[Dict, List]:
         """Get a single row from a table.
 
-        :param table:   Table to read
-        :param row:     Row to read
-        :param as_list: Return list instead of dictionary
-        :return:        Dictionary or List of table row
+        Args:
+            table:   Table to read
+            :param row:     Row to read
+            :param as_list: Return list instead of dictionary
 
-        Examples:
+        Returns:
+            (Union[dict, list]): Dictionary or List of table row
 
-        .. code-block:: robotframework
+        Example:
+            .. code-block:: robotframework
 
-            # returns the first row in the table
-            ${first}=    Get table row    ${orders}
+                # returns the first row in the table
+                ${first}=    Get table row    ${orders}
+
+                # returns the last row in the table
+                ${last}=      Get table row    ${orders}    -1    as_list=${TRUE}
 
-            # returns the last row in the table
-            ${last}=      Get table row    ${orders}    -1    as_list=${TRUE}
         """
         self._requires_table(table)
         values = table.get_row(row, as_list=as_list)
         return values
 
     def get_table_column(self, table: Table, column: Column) -> List:
         """Get all values for a single column in a table.
 
-        :param table:   Table to read
-        :param column:  Column to read
-        :return:        List of the rows in the selected column
+        Args:
+            table:   Table to read
+            column:  Column to read
+
+        Returns:
+            list: List of the rows in the selected column
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                ${emails}=    Get table column    ${users}    E-Mail Address
 
-            ${emails}=    Get table column    ${users}    E-Mail Address
         """
         self._requires_table(table)
         col = table.get_column(column, as_list=True)
         return col
 
     def set_table_row(self, table: Table, row: Index, values: Any):
         """Assign values to a row in the table.
 
-        :param table:   Table to modify
-        :param row:     Row to modify
-        :param values:  Value(s) to set
+        Args:
+            table:   Table to modify
+            row:     Row to modify
+            values:  Value(s) to set
 
         The ``values`` can either be a list of values, or a dictionary
         where the keys match current column names. Values for unknown
         keys are discarded.
 
         It can also be a single value that is set for all columns.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                ${columns}=  Create list     One  Two  Three
+                ${table}=    Create table    columns=${columns}
 
-            ${columns}=  Create list     One  Two  Three
-            ${table}=    Create table    columns=${columns}
+                ${values}=   Create list     1  2  3
+                Set table row    ${table}    0    ${values}
 
-            ${values}=   Create list     1  2  3
-            Set table row    ${table}    0    ${values}
+                ${values}=   Create dictionary    One=1  Two=2  Three=3
+                Set table row    ${table}    1    ${values}
 
-            ${values}=   Create dictionary    One=1  Two=2  Three=3
-            Set table row    ${table}    1    ${values}
+                Set table row    ${table}    2    ${NONE}
 
-            Set table row    ${table}    2    ${NONE}
         """
         self._requires_table(table)
         table.set_row(row, values)
 
     def set_table_column(self, table: Table, column: Column, values: Any):
         """Assign values to a column in the table.
 
-        :param table:   Table to modify
-        :param column:  Column to modify
-        :param values:  Value(s) to set
+        Args:
+            table:   Table to modify
+            column:  Column to modify
+            values:  Value(s) to set
 
         The ``values`` can either be a list of values, one for each row, or
         one single value that is set for all rows.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Set different value for each row (sizes must match)
+                ${ids}=    Create list    1  2  3  4  5
+                Set table column    ${users}    userId    ${ids}
 
-            # Set different value for each row (sizes must match)
-            ${ids}=    Create list    1  2  3  4  5
-            Set table column    ${users}    userId    ${ids}
+                # Set the same value for all rows
+                Set table column    ${users}    email     ${NONE}
 
-            # Set the same value for all rows
-            Set table column    ${users}    email     ${NONE}
         """
         self._requires_table(table)
         table.set_column(column, values)
 
     def pop_table_row(
         self, table: Table, row: Optional[Index] = None, as_list: bool = False
     ) -> Union[Dict, List]:
         """Remove row from table and return it.
 
-        :param table:   Table to modify
-        :param row:     Row index, pops first row if none given
-        :param as_list: Return list instead of dictionary
-        :return:        Dictionary or List of the removed, popped, row
+        Args:
+            table:   Table to modify
+            row:     Row index, pops first row if none given
+            as_list: Return list instead of dictionary
+
+        Returns:
+            (Union[dict, list]): Dictionary or List of the removed, popped, row
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Pop the firt row in the table and discard it
+                Pop table row    ${orders}
 
-            # Pop the firt row in the table and discard it
-            Pop table row    ${orders}
+                # Pop the last row in the table and store it
+                ${row}=      Pop table row    ${data}    -1    as_list=${TRUE}
 
-            # Pop the last row in the table and store it
-            ${row}=      Pop table row    ${data}    -1    as_list=${TRUE}
         """
         self._requires_table(table)
         row = if_none(row, table.index[0])
 
         values = table.get_row(row, as_list=as_list)
         table.delete_rows(row)
         return values
 
     def pop_table_column(
         self, table: Table, column: Optional[Column] = None
     ) -> Union[Dict, List]:
         """Remove column from table and return it.
 
-        :param table:   Table to modify
-        :param column:  Column to remove
-        :return:        Dictionary or List of the removed, popped, column
+        Args:
+            table:   Table to modify
+            column:  Column to remove
+
+        Returns:
+            (Union[dict, list]): Dictionary or List of the removed, popped, column
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Remove column from table and discard it
+                Pop table column    ${users}   userId
 
-            # Remove column from table and discard it
-            Pop table column    ${users}   userId
+                # Remove column from table and iterate over it
+                ${ids}=    Pop table column    ${users}    userId
+                FOR    ${id}    IN    @{ids}
+                    Log    User id: ${id}
+                END
 
-            # Remove column from table and iterate over it
-            ${ids}=    Pop table column    ${users}    userId
-            FOR    ${id}    IN    @{ids}
-                Log    User id: ${id}
-            END
         """
         self._requires_table(table)
         column: Column = if_none(column, table.columns[0])
 
         values = self.get_table_column(table, column)
         table.delete_columns(column)
         return values
 
     def get_table_slice(
         self, table: Table, start: Optional[Index] = None, end: Optional[Index] = None
     ) -> Union[Table, List[List]]:
         """Return a new Table from a range of given Table rows.
 
-        :param table:   Table to read from
-        :param start:   Start index (inclusive)
-        :param start:   End index (exclusive)
-        :return:        Table object of the selected rows
+        Args:
+            table:   Table to read from
+            start:   Start index (inclusive)
+            start:   End index (exclusive)
+
+        Returns:
+            (Union[Table, list[list]]): Table object of the selected rows
 
         If ``start`` is not defined, starts from the first row.
         If ``end`` is not defined, stops at the last row.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Get all rows except first five
+                ${slice}=    Get table slice    ${table}    start=5
 
-            # Get all rows except first five
-            ${slice}=    Get table slice    ${table}    start=5
+                # Get rows at indexes 5, 6, 7, 8, and 9
+                ${slice}=    Get table slice    ${table}    start=5    end=10
 
-            # Get rows at indexes 5, 6, 7, 8, and 9
-            ${slice}=    Get table slice    ${table}    start=5    end=10
+                # Get all rows except last five
+                ${slice}=    Get table slice    ${table}    end=-5
 
-            # Get all rows except last five
-            ${slice}=    Get table slice    ${table}    end=-5
         """
         self._requires_table(table)
         return table.get_slice(start, end)
 
     def set_row_as_column_names(self, table: Table, row: Index):
         """Set existing row as names for columns.
 
-        :param table: Table to modify
-        :param row:   Row to use as column names
+        Args:
+            table: Table to modify
+            row:   Row to use as column names
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Set the column names based on the first row
+                Set row as column names    ${table}    0
 
-            # Set the column names based on the first row
-            Set row as column names    ${table}    0
         """
         values = self.pop_table_row(table, row, as_list=True)
         table.columns = values
 
     def table_head(
         self, table: Table, count: int = 5, as_list: bool = False
     ) -> Union[Table, List[List]]:
         """Return first ``count`` rows from a table.
 
-        :param table:   Table to read from
-        :param count:   Number of lines to read
-        :param as_list: Return list instead of Table
-        :return:        Return Table object or List of the selected rows
+        Args:
+            table:   Table to read from
+            count:   Number of lines to read
+            as_list: Return list instead of Table
+        Returns:
+            (Union[Table, List[List]]): Return Table object or List of the selected rows
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Get the first 10 employees
+                ${first}=    Table head    ${employees}    10
 
-            # Get the first 10 employees
-            ${first}=    Table head    ${employees}    10
         """
         self._requires_table(table)
         return table.head(count, as_list)
 
     def table_tail(
         self, table: Table, count: int = 5, as_list: bool = False
     ) -> Union[Table, List[List]]:
         """Return last ``count`` rows from a table.
 
-        :param table:   Table to read from
-        :param count:   Number of lines to read
-        :param as_list: Return list instead of Table
-        :return:        Return Table object or List of the selected rows
+        Args:
+            table:   Table to read from
+            count:   Number of lines to read
+            as_list: Return list instead of Table
+
+        Returns:
+            (Union[Table, List[List]]): Return Table object or List of the selected rows
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Get the last 10 orders
+                ${latest}=    Table tail    ${orders}    10
 
-            # Get the last 10 orders
-            ${latest}=    Table tail    ${orders}    10
         """
         self._requires_table(table)
         return table.tail(count, as_list)
 
     def get_table_cell(self, table: Table, row: Index, column: Column) -> Any:
         """Get a cell value from a table.
 
-        :param table:   Table to read from
-        :param row:     Row of cell
-        :param column:  Column of cell
-        :return:        Cell value
+        Args:
+            table:   Table to read from
+            row:     Row of cell
+            column:  Column of cell
+
+        Returns:
+            (Any): Cell value
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Get the value in the first row and first column
+                Get table cell    ${table}    0    0
 
-            # Get the value in the first row and first column
-            Get table cell    ${table}    0    0
+                # Get the value in the last row and first column
+                Get table cell    ${table}   -1    0
 
-            # Get the value in the last row and first column
-            Get table cell    ${table}   -1    0
+                # Get the value in the last row and last column
+                Get table cell    ${table}   -1    -1
 
-            # Get the value in the last row and last column
-            Get table cell    ${table}   -1    -1
+                # Get the value in the third row and column "Name"
+                Get table cell    ${table}    2    Name
 
-            # Get the value in the third row and column "Name"
-            Get table cell    ${table}    2    Name
         """
         self._requires_table(table)
         return table.get_cell(row, column)
 
     def set_table_cell(self, table: Table, row: Index, column: Column, value: Any):
         """Set a cell value in a table.
 
-        :param table:   Table to modify to
-        :param row:     Row of cell
-        :param column:  Column of cell
-        :param value:   Value to set
+        Args:
+            table:   Table to modify to
+            row:     Row of cell
+            column:  Column of cell
+            value:   Value to set
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Set the value in the first row and first column to "First"
+                Set table cell    ${table}    0    0       First
 
-            # Set the value in the first row and first column to "First"
-            Set table cell    ${table}    0    0       First
+                # Set the value in the last row and first column to "Last"
+                Set table cell    ${table}   -1    0       Last
 
-            # Set the value in the last row and first column to "Last"
-            Set table cell    ${table}   -1    0       Last
+                # Set the value in the last row and last column to "Corner"
+                Set table cell    ${table}   -1    -1       Corner
 
-            # Set the value in the last row and last column to "Corner"
-            Set table cell    ${table}   -1    -1       Corner
+                # Set the value in the third row and column "Name" to "Unknown"
+                Set table cell    ${table}    2    Name    Unknown
 
-            # Set the value in the third row and column "Name" to "Unknown"
-            Set table cell    ${table}    2    Name    Unknown
         """
         self._requires_table(table)
         table.set_cell(row, column, value)
 
-    def find_table_rows(self, table: Table, column: Column, operator: str, value: Any):
+    def find_table_rows(
+        self, table: Table, column: Column, operator: str, value: Any
+    ) -> Table:
         """Find all the rows in a table which match a condition for a given column.
 
-        :param table: Table to search into.
-        :param column: Name or position of the column to compare with.
-        :param operator: Comparison operator used with every cell value on the
+        Args:
+            table: Table to search into.
+            column: Name or position of the column to compare with.
+            operator: Comparison operator used with every cell value on the
             specified column.
-        :param value: Value to compare against.
-        :return: New `Table` object containing all the rows matching the condition.
+            value: Value to compare against.
+
+        Returns:
+            Table: New `Table` object containing all the rows matching the condition.
 
         Supported operators:
 
         ============ ========================================
         Operator     Description
         ============ ========================================
         >            Cell value is larger than
@@ -1611,22 +1662,22 @@
         in           Cell value is in given value
         not in       Cell value is not in given value
         ============ ========================================
 
         Returns the matches as a new `Table` instance.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Find all rows where price is over 200
+                @{rows} =    Find table rows    ${table}    Price  >  ${200}
 
-            # Find all rows where price is over 200
-            @{rows} =    Find table rows    ${table}    Price  >  ${200}
+                # Find all rows where the status does not contain "removed"
+                @{rows} =    Find table rows    ${table}    Status  not contains  removed
 
-            # Find all rows where the status does not contain "removed"
-            @{rows} =    Find table rows    ${table}    Status  not contains  removed
         """
         self._requires_table(table)
 
         condition = to_condition(operator, value)
 
         matches = []
         for index in table.index:
@@ -1637,102 +1688,109 @@
         return table.get_table(matches)
 
     def sort_table_by_column(
         self, table: Table, column: Column, ascending: bool = True
     ):
         """Sort a table in-place according to ``column``.
 
-        :param table:       Table to sort
-        :param column:      Column to sort with
-        :param ascending:   Table sort order
+        Args:
+            table:       Table to sort
+            column:      Column to sort with
+            ascending:   Table sort order
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Sorts the `order_date` column ascending
+                Sort table by column    ${orders}    order_date
 
-            # Sorts the `order_date` column ascending
-            Sort table by column    ${orders}    order_date
+                # Sorts the `order_date` column descending
+                Sort table by column    ${orders}    order_date    ascending=${FALSE}
 
-            # Sorts the `order_date` column descending
-            Sort table by column    ${orders}    order_date    ascending=${FALSE}
         """
         self._requires_table(table)
         table.sort_by_column(column, ascending=ascending)
 
     def group_table_by_column(self, table: Table, column: Column) -> List[Table]:
         """Group a table by ``column`` and return a list of grouped Tables.
 
-        :param table:   Table to use for grouping
-        :param column:  Column which is used as grouping criteria
-        :return:        List of Table objects
+        Args:
+            table:   Table to use for grouping
+            column:  Column which is used as grouping criteria
+
+        Returns:
+            (List[Table]): List of Table objects
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Groups rows of matching customers from the `customer` column
+                # and returns the groups or rows as Tables
+                @{groups}=    Group table by column    ${orders}    customer
+                # An example of how to use the List of Tables once returned
+                FOR    ${group}    IN    @{groups}
+                    # Process all orders for the customer at once
+                    Process order    ${group}
+                END
 
-            # Groups rows of matching customers from the `customer` column
-            # and returns the groups or rows as Tables
-            @{groups}=    Group table by column    ${orders}    customer
-            # An example of how to use the List of Tables once returned
-            FOR    ${group}    IN    @{groups}
-                # Process all orders for the customer at once
-                Process order    ${group}
-            END
         """
         self._requires_table(table)
         groups = table.group_by_column(column)
         self.logger.info("Found %s groups", len(groups))
         return groups
 
     def filter_table_by_column(
         self, table: Table, column: Column, operator: str, value: Any
     ):
-        """Remove all rows where column values don't match the
-        given condition.
+        """Remove all rows where column values don't match the given condition.
 
-        :param table:     Table to filter
-        :param column:    Column to filter with
-        :param operator:  Filtering operator, e.g. >, <, ==, contains
-        :param value:     Value to compare column to (using operator)
+        Args:
+            table:     Table to filter
+            column:    Column to filter with
+            operator:  Filtering operator, e.g. >, <, ==, contains
+            value:     Value to compare column to (using operator)
 
         See the keyword ``Find table rows`` for all supported operators
         and their descriptions.
 
         The filtering will be done in-place.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Only accept prices that are non-zero
+                Filter table by column    ${table}   price  !=  ${0}
 
-            # Only accept prices that are non-zero
-            Filter table by column    ${table}   price  !=  ${0}
+                # Remove uwnanted product types
+                @{types}=    Create list    Unknown    Removed
+                Filter table by column    ${table}   product_type  not in  ${types}
 
-            # Remove uwnanted product types
-            @{types}=    Create list    Unknown    Removed
-            Filter table by column    ${table}   product_type  not in  ${types}
         """
         self._requires_table(table)
 
         condition = to_condition(operator, value)
 
         before = len(table)
         table.filter_by_column(column, condition)
         after = len(table)
 
         self.logger.info("Filtered %d rows", after - before)
 
     def filter_table_with_function(self, table: Table, func: Callable, *args):
-        """Run a keyword for each row of a table, then remove all rows where the called
+        """Filters the table rows with the given func.
+
+        Run a function for each row of a table, then remove all rows where the called
         keyword returns a falsy value.
 
         Can be used to create custom RF keyword based filters.
 
-        :param table: Table to modify.
-        :param func: Function used as filter.
-        :param args: Additional keyword arguments to be passed. (optional)
+        Args:
+            table: Table to modify.
+            func: Function used as filter.
+            args: Additional keyword arguments to be passed. (optional)
 
         The row object will be given as the first argument to the filtering keyword.
         """
         self._requires_table(table)
 
         def condition(row: Row) -> bool:
             return func(row, *args)
@@ -1740,81 +1798,85 @@
         before = len(table)
         table.filter_all(condition)
         after = len(table)
 
         self.logger.info("Removed %d row(s)", before - after)
 
     def map_column_values(self, table: Table, column: Column, func: Callable, *args):
-        """Run a keyword for each cell in a given column, and replace its content with
+        """Maps given function to column values.
+
+        Run a function for each cell in a given column, and replace its content with
         the return value.
 
         Can be used to easily convert column types or values in-place.
 
-        :param table: Table to modify.
-        :param column: Column to modify.
-        :param func: Mapping function.
-        :param args: Additional keyword arguments. (optional)
+        Args:
+            table: Table to modify.
+            column: Column to modify.
+            func: Mapping function.
+            args: Additional keyword arguments. (optional)
 
         The cell value will be given as the first argument to the mapping keyword.
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Convert all columns values to a different type
+                Map column values    ${table}    Price    Convert to integer
 
-            # Convert all columns values to a different type
-            Map column values    ${table}    Price    Convert to integer
+                # Look up values with a custom keyword
+                Map column values    ${table}    User     Map user ID to name
 
-            # Look up values with a custom keyword
-            Map column values    ${table}    User     Map user ID to name
         """
         self._requires_table(table)
 
         values = []
         for index in table.index:
             cell = table.get_cell(index, column)
             output = func(cell, *args)
             values.append(output)
 
         table.set_column(column, values)
 
     def filter_empty_rows(self, table: Table):
         """Remove all rows from a table which have only ``None`` values.
 
-        :param table:   Table to filter
+        Args:
+            table:   Table to filter
 
         The filtering will be done in-place.
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                Filter empty rows    ${table}
 
-            Filter empty rows    ${table}
         """
         self._requires_table(table)
 
         empty = []
         for idx, row in table.iter_lists():
             if all(value is None for value in row):
                 empty.append(idx)
 
         table.delete_rows(empty)
 
     def trim_empty_rows(self, table: Table):
-        """Remove all rows from the *end* of a table
-        which have only ``None`` as values.
+        """Remove all rows from the *end* of a table, which have only ``None`` as values.
 
-        :param table:    Table to filter
+        Args:
+            table:    Table to filter
 
         The filtering will be done in-place.
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                Trim empty rows    ${table}
 
-            Trim empty rows    ${table}
         """
         self._requires_table(table)
 
         empty = []
         for idx in reversed(table.index):
             row = table[idx]
             if any(value is not None for value in row):
@@ -1822,27 +1884,28 @@
             empty.append(idx)
 
         table.delete_rows(empty)
 
     def trim_column_names(self, table: Table):
         """Remove all extraneous whitespace from column names.
 
-        :param table:    Table to filter
+        Args:
+            table:    Table to filter
 
         The filtering will be done in-place.
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # This example will take colums such as:
+                # "One", "Two ", "  Three "
+                # and trim them to become the below:
+                # "One", "Two", "Three"
+                Trim column names     ${table}
 
-            # This example will take colums such as:
-            # "One", "Two ", "  Three "
-            # and trim them to become the below:
-            # "One", "Two", "Three"
-            Trim column names     ${table}
         """
         self._requires_table(table)
         table.columns = [
             column.strip() if isinstance(column, str) else column
             for column in table.columns
         ]
 
@@ -1854,52 +1917,54 @@
         dialect: Optional[Union[str, Dialect]] = None,
         delimiters: Optional[str] = None,
         column_unknown: str = "Unknown",
         encoding: Optional[str] = None,
     ) -> Table:
         """Read a CSV file as a table.
 
-        :param path:            Path to CSV file
-        :param header:          CSV file includes header
-        :param columns:         Names of columns in resulting table
-        :param dialect:         Format of CSV file
-        :param delimiters:      String of possible delimiters
-        :param column_unknown:  Column name for unknown fields
-        :param encoding:        Text encoding for input file,
+        Args:
+            path:            Path to CSV file
+            header:          CSV file includes header
+            columns:         Names of columns in resulting table
+            dialect:         Format of CSV file
+            delimiters:      String of possible delimiters
+            column_unknown:  Column name for unknown fields
+            encoding:        Text encoding for input file,
                                 uses system encoding by default
-        :return:                Table object
+        Returns:
+            Table: Table object
 
-        By default attempts to deduce the CSV format and headers
+        By default, attempts to deduce the CSV format and headers
         from a sample of the input file. If it's unable to determine
         the format automatically, the dialect and header will
         have to be defined manually.
 
         Builtin ``dialect`` values are ``excel``, ``excel-tab``, and ``unix``,
         and ``header`` is boolean argument (``True``/``False``). Optionally a
         set of valid ``delimiters`` can be given as a string.
 
         The ``columns`` argument can be used to override the names of columns
         in the resulting table. The amount of columns must match the input
         data.
 
         If the source data has a header and rows have more fields than
         the header defines, the remaining values are put into the column
-        given by ``column_unknown``. By default it has the value "Unknown".
+        given by ``column_unknown``. By default, it has the value "Unknown".
 
         Examples:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                # Source dialect is deduced automatically
+                ${table}=    Read table from CSV    export.csv
+                Log   Found columns: ${table.columns}
+
+                # Source dialect is known and given explicitly
+                ${table}=    Read table from CSV    export-excel.csv    dialect=excel
+                Log   Found columns: ${table.columns}
 
-            # Source dialect is deduced automatically
-            ${table}=    Read table from CSV    export.csv
-            Log   Found columns: ${table.columns}
-
-            # Source dialect is known and given explicitly
-            ${table}=    Read table from CSV    export-excel.csv    dialect=excel
-            Log   Found columns: ${table.columns}
         """
         sniffer = csv.Sniffer()
         with open(path, newline="", encoding=encoding) as fd:
             sample = fd.readline()
 
         if dialect is None:
             dialect_name = sniffer.sniff(sample, delimiters)
@@ -1938,30 +2003,31 @@
         header: bool = True,
         dialect: Union[str, Dialect] = Dialect.Excel,
         encoding: Optional[str] = None,
         delimiter: Optional[str] = ",",
     ):
         """Write a table as a CSV file.
 
-        :param table:    Table to write
-        :param path:     Path to write to
-        :param header:   Write columns as header to CSV file
-        :param dialect:  The format of output CSV
-        :param encoding: Text encoding for output file,
+        Args:
+            table:    Table to write
+            path:     Path to write to
+            header:   Write columns as header to CSV file
+            dialect:  The format of output CSV
+            encoding: Text encoding for output file,
                          uses system encoding by default
-        :param delimiter: Delimiter character between columns
+            delimiter: Delimiter character between columns
 
         Builtin ``dialect`` values are ``excel``, ``excel-tab``, and ``unix``.
 
         Example:
+            .. code-block:: robotframework
 
-        .. code-block:: robotframework
+                ${sheet}=    Read worksheet as table    orders.xlsx    header=${TRUE}
+                Write table to CSV    ${sheet}    output.csv
 
-            ${sheet}=    Read worksheet as table    orders.xlsx    header=${TRUE}
-            Write table to CSV    ${sheet}    output.csv
         """
         self._requires_table(table)
 
         if isinstance(dialect, Dialect):
             dialect_name = dialect.value
         else:
             dialect_name = dialect
```

### Comparing `robocorp_excel-0.1.0/src/robo/libs/excel/workbook.py` & `robocorp_excel-0.2.0/src/robocorp/excel/workbook.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-import logging
 import pathlib
+from io import BytesIO
 from typing import Any, List, Optional, Union
-from typing_extensions import Literal
 
-from robo.libs.excel._types import PathType
-from robo.libs.excel._worksheet import Worksheet
-from robo.libs.excel._workbooks import XlsWorkbook, XlsxWorkbook
+from robocorp.excel._types import PathType
+from robocorp.excel.worksheet import Worksheet
+from robocorp.excel._workbooks import XlsWorkbook, XlsxWorkbook
 
 
 class Workbook:
+    """Manager class for both .xls and .xlsx Excel files."""
+
     def __init__(self, excel: Union[XlsWorkbook, XlsxWorkbook]):
         # Internal API, for users there is create_ and open_ workbook functions
         self.excel = excel
 
-    def save(self, name: PathType):
+    def save(self, name: Union[PathType, BytesIO], overwrite=True):
         # files.save_workbook()
+        if not isinstance(name, BytesIO):
+            if not overwrite and pathlib.Path(name).exists():
+                raise FileExistsError
+        self.excel.validate_content()
         self.excel.save(name)
 
     def close(self):
         # Could also be a context manager and auto close
         # files.close_workbook()
         pass
 
@@ -38,19 +43,22 @@
         content: Optional[Any] = None,
         exist_ok: Optional[bool] = False,
         header: Optional[bool] = False,
     ):
         # files.create_worksheet()
         # TODO: original code: https://github.com/robocorp/rpaframework/blob/dec0053a3aa34da20232f63e1b26e21df98e59e8/packages/main/src/RPA/Excel/Files.py#L539
         # TODO: implement content and header
-        if exist_ok:
-            if name in self.list_worksheets():
-                return Worksheet(self, name)
+        if name in self.list_worksheets():
+            if not exist_ok:
+                raise ValueError(f"Duplicate worksheet name '{name}'")
+            return Worksheet(self, name)
 
         self.excel.create_worksheet(name)
+        if content:
+            self.excel.append_worksheet(name, content, header)
         return Worksheet(self, name)
 
     # files.list_worksheets()
     def list_worksheets(self) -> List[str]:
         return self.excel.sheetnames
 
     def worksheet_exists(self, sheet: Union[str, int]) -> bool:
```

### Comparing `robocorp_excel-0.1.0/PKG-INFO` & `robocorp_excel-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: robocorp-excel
-Version: 0.1.0
+Version: 0.2.0
 Summary: Robocorp Excel automation library
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
+Requires-Dist: pillow (>=9.1.1,<10.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Requires-Dist: xlutils (>=2.0.0,<3.0.0)
 Requires-Dist: xlwt (>=1.3.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Robocorp excel library
```

