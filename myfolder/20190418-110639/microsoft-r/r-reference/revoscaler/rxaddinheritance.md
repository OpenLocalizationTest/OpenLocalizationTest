<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxaddinheritance.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f170de49768790b83dedc39eb7ba758bcda824379.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">170de49768790b83dedc39eb7ba758bcda824379</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxaddinheritance.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxAddInheritance function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Add a specific S3 class to the class of a compatible object.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxAddInheritance, rxAddInheritance.default, rxAddInheritance.rxDTree, models, tree, classif, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxAddInheritance: Add Inheritance to Compatible Objects</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Add a specific S3 class to the <ph id="ph1">`"class"`</ph> of a compatible object.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>the object to which inheritance is to be added.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Specifically, for <ph id="ph1">`rxAddInheritance.rxDTree`</ph>, an object of class <ph id="ph2">`rxDTree`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>the class to be inherited from.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Specifically, for <ph id="ph1">`rxAddInheritance.rxDTree`</ph>, the class <ph id="ph2">`"rpart"`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to other methods.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxAddInheritance`</ph> function is designed to be a general way to add inheritance to S3 objects that are compatible with the class for which inheritance is to be added.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Note, however, that this approach is exactly as dangerous and error-prone as simply calling <ph id="ph1">`class(x) &lt;- c(class(x), inheritanceClass)`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>It is expected that classes that are designed to mimic existing R classes, but not rely on them, will have their own specific <ph id="ph1">`rxAddInheritance`</ph> methods to add the R class inheritance on request.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In the case of <ph id="ph1">`rxDTree`</ph> objects, these were designed to be compatible with the <ph id="ph2">`"rpart"`</ph> class.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>so adding <bpt id="p1">**</bpt>rpart<ept id="p1">**</ept> inheritance is guaranteed to work.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The original object, modified to include <ph id="ph1">`inheritanceClass`</ph> as part of its <ph id="ph2">`"class"`</ph> attribute.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In the case of <ph id="ph1">`rxDTree`</ph> objects, the object may also be modified to include the <ph id="ph2">`functions`</ph> component if it was previously <ph id="ph3">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDTree<ept id="p1">](rxDTree.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>