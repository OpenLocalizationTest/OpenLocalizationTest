<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxtweedie.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338abcba3df689503f7e1510c9f0f2c30621c836887f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bcba3df689503f7e1510c9f0f2c30621c836887f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxtweedie.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxTweedie function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Produces a dummy generalized linear model family object that can be used with rxGlm to fit  Tweedie generalized linear regression models.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This does NOT produce a full family object, but gives  rxGlm enough information to call a C++ implementation that fits a Tweedie model.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The excellent  R package <bpt id="p1">**</bpt>tweedie<ept id="p1">**</ept> by Gordon Smyth does provide a full Tweedie family object, and that can also be  used with rxGlm.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxTweedie, regression</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>rxTweedie: Tweedie Generalized Linear Models</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Produces a dummy generalized linear model family object that can be used with <ph id="ph1">`rxGlm`</ph> to fit Tweedie generalized linear regression models.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This does NOT produce a full family object, but gives <ph id="ph1">`rxGlm`</ph> enough information to call a C++ implementation that fits a Tweedie model.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The excellent R package <bpt id="p1">**</bpt>tweedie<ept id="p1">**</ept> by Gordon Smyth does provide a full Tweedie family object, and that can also be used with <ph id="ph1">`rxGlm`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>index of power variance function.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>index of power link function.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`link.power`</ph> to <ph id="ph2">`0`</ph>  produces a <ph id="ph3">`log`</ph> link function.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Setting it to <ph id="ph1">`1`</ph> is the identity link.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The default is a canonical link  equal to</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This provides a way to specify the var.power and the link.power arguments to the Tweedie distribution for <ph id="ph1">`rxGlm`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Peter K Dunn (2011).</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>tweedie: Tweedie exponential family models.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>R package version 2.1.1.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>rxGlm</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>