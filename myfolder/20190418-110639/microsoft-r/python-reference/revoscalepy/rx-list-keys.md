<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-list-keys.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f4501257781c83902bec6dcf2e91112a3bf9d6140.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4501257781c83902bec6dcf2e91112a3bf9d6140</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-list-keys.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_list_keys: Manage objects in ODBC Data Sources (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Retrieves object keys from ODBC data sources.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>keys</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_list_keys</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Retrieves object keys from ODBC data sources.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Enumerates all keys or versions for a given key, depending on the parameters.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>When key is None, the function enumerates all unique keys in the table.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Otherwise, it enumerates all versions for the given key.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Returns a single column data frame.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The key and the version should be of some SQL character type (CHAR, VARCHAR, NVARCHAR, etc.) supported by the data source.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The value column should be a binary type (VARBINARY for instance).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Some conversions to other types might work, however, they are dependent on the ODBC driver and on the underlying package functions.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>value</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The object being stored into the data source.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>key</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>A character string identifying the object.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The intended use is for the key+version to be unique.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>version</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>None or a character string which carries the version of the object.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Combined with key identifies the object.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>key_name</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Character string specifying the column name for the key in the underlying table.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>value_name</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Character string specifying the column name for the objects in the underlying table.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>version_name</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Character string specifying the column name for the version in the underlying table.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>rx_read_object returns an object.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>rx_write_object and rx_delete_object return bool, True on success.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>rx_list_keys returns a single column data frame containing strings.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>