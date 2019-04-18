<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxtransform.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9262dfec736bd5a2c592042268efec2e464ddf1a302.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2dfec736bd5a2c592042268efec2e464ddf1a302</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxtransform.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxTransform function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Description of the recommended method for creating <bpt id="p1">*</bpt>on the fly<ept id="p1">*</ept> variables.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxTransform, transformFunc, transformVars, models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxTransform: Dynamic Variable Transformation Functions</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description of the recommended method for creating <bpt id="p1">*</bpt>on the fly<ept id="p1">*</ept> variables.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Analytical functions within the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package use a formal transformation function framework for generating <bpt id="p2">*</bpt>on the fly<ept id="p2">*</ept> variables as opposed to the traditional R method of including transformations directly in a <ph id="ph1">`formula`</ph> statement.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> approach is to use the following analytical function arguments to create new named variables that can be referenced by name within a <ph id="ph1">`formula`</ph> statement:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`transformFunc`</ph>: R function whose first argument and return value are named R lists with equal length vector elements.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The output list can contain modifications to the input elements as well as newly named elements.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>R lists, instead of R data frames, are used to minimize function execution timings, implying that row name information will not be available during calculations.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`transformVars`</ph>: character vector selecting the names of the variables to be represented as list elements for the input to <ph id="ph2">`transformFunc`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In application, the <ph id="ph1">`transformFunc`</ph> argument is analogous to the <ph id="ph2">`FUN`</ph> argument in R's apply, lapply, etc. functions.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Just as with the <ph id="ph1">`*apply`</ph> functions, the <ph id="ph2">`transformFunc`</ph> function does not receive results from previous chunks as input and so an external mechanism is required to carry over results from one chunk to the next.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Additional information variables are available for use within a transformation function when working in a local compute context:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxStartRow`</ph>: the row number from the original data set of the first row in the chunk of data that is being processed.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxChunkNum`</ph>: the chunk number of the data being  processed, set to 0 if a test sample of data is being processed.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>For example, if there are 10 blocks of data in an .xdf file, and <ph id="ph1">`blocksPerRead`</ph> is set to 2, there will be 5 chunks of data.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxNumRows`</ph>: the number of rows in the current chunk.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxReadFileName`</ph>: character string containing the name of the .xdf file being processed.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxIsTestChunk`</ph>: logical set to <ph id="ph2">`TRUE`</ph> if the chunk of data being processed is a test sample of data.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxIsPrediction`</ph>: logical set to <ph id="ph2">`TRUE`</ph> if the chunk of data being processed being used in a prediction rather than a model estimation.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxTransformEnvir`</ph>: environment containing the data specified in <ph id="ph2">`transformObjects`</ph>, which is also the parent environment to the transformation functions.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Three functions are also available for use within transformation functions that facilitate the interaction with <ph id="ph1">`transformObjects`</ph> objects packed into transformation function environment (<ph id="ph2">`.rxTransformEnvir`</ph>):</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxGet(objName)`</ph>: Get the value of an object in the transform environment,  e.g., <ph id="ph2">`.rxGet("myObject")`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxSet(objName, objValue)`</ph>: Set the value of an object in the transform environment,  e.g., <ph id="ph2">`.rxSet("myObject", pi)`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`.rxModify(objName, ..., FUN = "+")`</ph>: Modify the value of an object in the transform environment by applying to the current value a specified function, <ph id="ph2">`FUN`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The first argument passed (behind the scenes)  to <ph id="ph1">`FUN`</ph> is always the current value of <ph id="ph2">`"objName"`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The ellipsis argument ( ...) denotes additional  arguments passed to <ph id="ph1">`FUN`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>By default, <ph id="ph1">`FUN = "+"`</ph>, the addition operator.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>e.g.,</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Increment the current value of "myObject" by 2:<ph id="ph1">`.rxModify("myObject", 2)`</ph></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Decrement the current value of "myObject" by 4:<ph id="ph1">`.rxModify("myObject", 4, FUN = "-")`</ph></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Convert "myObject", assumed to be a vector, to a factor with  specified levels:<ph id="ph1">`.rxModify("myObject", levels = 1:5, exclude = 6:10, FUN = "factor")`</ph></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>, <bpt id="p2">[</bpt>rxTransform<ept id="p2">](rxTransform.md)</ept>, <bpt id="p3">[</bpt>rxCrossTabs<ept id="p3">](rxCrossTabs.md)</ept>, <bpt id="p4">[</bpt>rxCube<ept id="p4">](rxCube.md)</ept>, <bpt id="p5">[</bpt>rxLinMod<ept id="p5">](rxLinMod.md)</ept>, <bpt id="p6">[</bpt>rxLogit<ept id="p6">](rxLogit.md)</ept>, <bpt id="p7">[</bpt>rxSummary<ept id="p7">](rxSummary.md)</ept>, <bpt id="p8">[</bpt>rxDataStep<ept id="p8">](rxDataStep.md)</ept>, <bpt id="p9">[</bpt>rxImport<ept id="p9">](rxImport.md)</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>