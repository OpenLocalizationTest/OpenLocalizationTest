<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxwriteobject.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e828a621bcf069b0e4a08e5d3a0856c77abdc4af3.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">828a621bcf069b0e4a08e5d3a0856c77abdc4af3</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxwriteobject.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxWriteObject function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Store/Retrieve R objects to/from ODBC data sources.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The APIs are modelled after a simple key value store.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>These are generic APIs and if the ODBC data source isn't specified in the argument, the function does serialization or deserialization of the R object with the specified compression if any.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxWriteObject, rxReadObject, rxDeleteObject, rxListKeys</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>rxWriteObject:  Manage R objects in ODBC Data Sources</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Store/Retrieve R objects to/from ODBC data sources.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The APIs are modelled after a simple key value store.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>These are generic APIs and if the ODBC data source isn't specified in the argument, the function does serialization or deserialization of the R object with the specified compression if any.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>an RxOdbcData object identifying the destination to which the data is to be written.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>an RxOdbcData object identifying the source from which the data is to be read.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>..</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>a raw R object to be read from.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>a character string identifying the R object to be written or read.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The intended use is  for the key+version to be unique.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>the R object being stored into the data source.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>or a character string which carries the version of the object.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Combined with key identifies the object.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>character string specifying the column name for the key in the underlying table.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>character string specifying the column name for the objects in the underlying table.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>character string specifying the column name for the version in the underlying table.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Dictates whether the object is to be serialized.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Only raw values are supported if serialization is off.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>character string defining the compression algorithm to use for memCompress.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Defines whether the object is to be de-serialized.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>character string defining the compression algorithm to use for memDecompress.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, <ph id="ph2">`rxWriteObject`</ph> first removes the key (or the key+version combination) before writing the new value.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Even when <ph id="ph1">`overwrite`</ph> is <ph id="ph2">`FALSE`</ph>, <ph id="ph3">`rxWriteObject`</ph> may still succeed if there is no database constraint (or index) enforcing uniqueness.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>to remove all objects from the data source.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the 'key' parameter is ignored.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>stores an R object into the specified ODBC data destination.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The R object to be written is identified by a key, and optionally, by a version (key+version).</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>By default, the object is serialized and compressed.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Returns <ph id="ph1">`TRUE`</ph> if successful.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If the ODBC data destination is not specified, the default implementation is dispatched which takes only the value of the R object with serialize and compress arguments.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>loads an R object from the ODBC data source (or from a raw) decompressing and unserializing it (by default) in the process.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Returns the R object.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If the data source parameter defines a query, the <ph id="ph1">`key`</ph> and the <ph id="ph2">`version`</ph> parameters are ignored.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>deletes an R object from the ODBC data source.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If there are multiple objects identified by the key/version combination, all are deleted.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>enumerates all keys or versions for a given key, depending on the parameters.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>When <ph id="ph1">`key`</ph> is <ph id="ph2">`NULL`</ph>, the function enumerates all unique keys in the table.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Otherwise, it enumerates all versions for the given key.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Returns a single column data frame.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`key`</ph> and the <ph id="ph2">`version`</ph> column should be of some SQL character type (<ph id="ph3">`CHAR`</ph>, <ph id="ph4">`VARCHAR`</ph>, <ph id="ph5">`NVARCHAR`</ph>, etc) supported by the data source.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`value`</ph> column should be a binary type (<ph id="ph2">`VARBINARY`</ph> for instance).</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Some conversions to other types might work, however, they are dependant on the ODBC driver and on the underlying package functions.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>returns an R object.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`rxDeleteObject`</ph> return logical, <ph id="ph2">`TRUE`</ph> on success.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>returns a single column data frame containing strings.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>