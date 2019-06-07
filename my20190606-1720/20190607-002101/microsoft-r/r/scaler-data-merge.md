<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="scaler-data-merge.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37aef00ac6755f9428b064cc76dceb05ccdeb9f2eb.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">aef00ac6755f9428b064cc76dceb05ccdeb9f2eb</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\scaler-data-merge.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Merge data in RevoScaleR using rxSort (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to merge data in a data frame or XDF file with the RevoScaleR rxMerge function.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to merge data using rxMerge in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Merging allows you to combine the information from two data sets into a third data set that can be used for subsequent analysis.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>One example is merging account information such as account number and billing address with transaction data such as account number and purchase details to create invoices.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In this case, the two files are merged on the common information, that is, the account number.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, you merge .xdf files and/or data frames with the rxMerge function.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This function supports a number of types of merge that are best illustrated by example.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The available types are as follows:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Inner</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Outer: left, right, and full</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>One-to-One</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Union</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>We describe each of these types in the following sections.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Inner merge</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>In the default inner merge type, one or more merge key columns is specified, and only those observations for which the specified key columns match exactly are combined to create new observations in the merged data set.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Suppose we have the following data from a dentist’s office:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>We can create a data frame with this information:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Suppose further we have the following information about procedures performed:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This data is put into another data frame:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Then we use rxMerge to create an inner merge matching on the columns <bpt id="p1">*</bpt>acct<ept id="p1">*</ept> and <bpt id="p2">*</bpt>patient:<ept id="p2">*</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Because the patient 1 in account 538 and patient 1 in account 1534 had no visits, they are omitted from the merged file.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Similarly, patient 2 in account 763 had a visit, but does not have any information in the accounts file, so it to is omitted from the merged data set.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Also, note that the two input data files are automatically sorted on the merge keys before merging.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Outer merge</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>There are three types of outer merge: left, right, and full.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>In a left outer merge, all the lines from the first file are present in the merged file, either matched with lines from the second file that match on the key columns, or if no match, filled out with missing values.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>A right outer merge is similar, except all the lines from the second file are present, either matched with matching lines from the first file or filled out with missings.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A full outer merge includes all lines in both files, either matched or filled out with missings.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>We can use the same dentist data to illustrate the various types of outer merge:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>One-to-one merge</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In the one-to-one merge type, the first observation in the first data set is paired with the first observation in the second data set to create the first observation in the merged data set, the second observation is paired with the second observation to create the second observation in the merged data set, and so on.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The data sets must have the same number of rows.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>It is equivalent to using <bpt id="p1">*</bpt>append=<ept id="p1">*</ept>"<bpt id="p2">*</bpt>cols<ept id="p2">*</ept>" in a data step.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For example, suppose our first data set contains three observations as follows:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Create a data frame with this data:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Suppose our second data set contains three different variables:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Create a data frame with this data:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>A one-to-one merge of these two data sets combines the columns from the two data sets into one data set:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Union merge</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A union merge is simply the concatenation of two files with the same set of variables.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>It is equivalent to using <bpt id="p1">*</bpt>append="rows"<ept id="p1">*</ept> in a data step.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Using the example from one-to-one merge, we rename the variables in the second data frame to be the same as in the first:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Then use a union merge:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Using rxMerge with .xdf files</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>You can use <bpt id="p1">**</bpt>rxMerge<ept id="p1">**</ept> with a combination of .xdf files or data frames.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>For example, you specify the two the paths for two input .xdf files as the <bpt id="p1">*</bpt>inData1<ept id="p1">*</ept> and <bpt id="p2">*</bpt>inData2<ept id="p2">*</ept> arguments, and the path to an output file as the <bpt id="p3">*</bpt>outFile<ept id="p3">*</ept> argument.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>As a simple example, we can stack two copies of the claims data using the union merge type as follows:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>A new .xdf file is created containing twice the number of rows of the original claims file.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You can also merge an .xdf file and data frame into a new .xdf file.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>For example, suppose that you would like to add a variable on state expenditure on education into each observation in the censusWorkers sample .xdf file.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>First, take a quick look at the state variable in the .xdf file:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>We can create a data frame with per capita educational expenditures for the same three states.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>(Note that because R alphabetizes factor levels by default, the factor levels in the data frame will be in the same order as those in the .xdf file).</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Now use rxMerge, matching by the variable <bpt id="p1">*</bpt>state:<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The new .xdf file has an additional variable, EducExp:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](~/what-is-machine-learning-server.md)</ept> <bpt id="p2">[</bpt>Install Machine Learning Server on Windows<ept id="p2">](~/install/machine-learning-server-windows-install.md)</ept></source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Linux</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Hadoop</source>
        </trans-unit></group></body></file></xliff>