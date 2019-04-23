<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxMissingValues.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a00e115b60f81cb4597fdd471db903cce905e14fd.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">00e115b60f81cb4597fdd471db903cce905e14fd</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxMissingValues.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxMissingValues: Provides different missing (NA) value constants for various scalar types (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>revoscalepy package uses Pandas dataframe as the abstraction to hold the data and manipulate it.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Pandas dataframe in turn uses NumPy ndarray to hold homogeneous data efficiently and provides fast access and manipulation functions on the ndarray.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Python and NumPy ndarray in particular only has numpy.NaN value for float types to indicate missing values.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>For other primitive datatypes, like int, there isn’t a missing value notation.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>If one uses Python’s None object to represent missing value in a series of data, say int, the whole ndarray’s dtype changes to object.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This makes dealing with data with missing values quite inefficient during processing.This class provides missing values for various NumPy data types which one can use to mark missing values in a sequence of data in ndarray.It provides missing value for following types:int8() for numpy.int8 with value of numpy.iinfo(np.int8).min  uint8() for numpy.uint8 with value of numpy.iinfo(np.uint8).max  int16() for numpy.int16 with value of numpy.iinfo(np.int16).min  uint16() for numpy.uint16 with value of numpy.iinfo(np.uint16).max  int32() for numpy.int32 with value of numpy.iinfo(np.int32).min  uint32() for numpy.uint32 with value of numpy.iinfo(np.uint32).max  int64() for numpy.int64 with value of numpy.iinfo(np.int64).min  uint64() for numpy.uint64 with value of numpy.iinfo(np.uint64).max  float16() for numpy.float16 with value of numpy.NaN  float32() for numpy.float32 with value of numpy.NaN  float64() for numpy.float64 with value of numpy.NaN</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>missing values, NA, NaN, nan, none, None</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>RxMissingValues</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>revoscalepy package uses Pandas dataframe as the abstraction to hold the data and manipulate it.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Pandas dataframe in turn uses NumPy ndarray to hold homogeneous data efficiently and provides fast access and manipulation functions on the ndarray.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Python and NumPy ndarray in particular only has numpy.NaN value for float types to indicate missing values.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For other primitive datatypes, like int, there isn’t a missing value notation.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If one uses Python’s None object to represent missing value in a series of data, say int, the whole ndarray’s dtype changes to object.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This makes dealing with data with missing values quite inefficient during processing.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This class provides missing values for various NumPy data types which one can use to mark missing values in a sequence of data in ndarray.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>It provides missing value for following types:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>int8() for numpy.int8 with value of numpy.iinfo(np.int8).min</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>uint8() for numpy.uint8 with value of numpy.iinfo(np.uint8).max</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>int16() for numpy.int16 with value of numpy.iinfo(np.int16).min</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>uint16() for numpy.uint16 with value of numpy.iinfo(np.uint16).max</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>int32() for numpy.int32 with value of numpy.iinfo(np.int32).min</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>uint32() for numpy.uint32 with value of numpy.iinfo(np.uint32).max</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>int64() for numpy.int64 with value of numpy.iinfo(np.int64).min</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>uint64() for numpy.uint64 with value of numpy.iinfo(np.uint64).max</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>float16() for numpy.float16 with value of numpy.NaN</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>float32() for numpy.float32 with value of numpy.NaN</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>float64() for numpy.float64 with value of numpy.NaN</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>