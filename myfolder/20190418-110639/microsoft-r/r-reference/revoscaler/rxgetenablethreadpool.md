<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetenablethreadpool.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fee6c0d1f9869a8242ad6c953ae03a4ca97d188f8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ee6c0d1f9869a8242ad6c953ae03a4ca97d188f8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetenablethreadpool.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetEnableThreadPool function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Gets or sets the current state of the thread pool (in a ready state or created ad hoc).</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetEnableThreadPool, rxSetEnableThreadPool, iteration</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetEnableThreadPool:  Get or Set Thread Pool State</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Gets or sets the current state of the thread pool (in a ready state or created ad hoc).</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Logical scalar.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the thread pool is instantiated and maintained in a ready state.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, threads are created in an ad hoc fashion; that is, they are created as needed.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxSetEnableThreadPool`</ph> function is used on Linux to turn the thread pool on and off.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>When the thread pool is on, it means that there exists a pool of threads that persist between calls, and are ready for processing.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>When the thread pool is off, it means that threads will be created on an ad hoc basis when calls requiring threading are made.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>By default, the thread pool is turned off to allow R processes that have loaded RevoScaleR to fork successfully as a mechanism for spawning (for example, by the <ph id="ph1">`multicore`</ph> package).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>On the Windows platform, the thread pool always persists, regardless of any user settings.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>There is a significant speed increase associated with having the thread pool ready and waiting to do work.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If you are sure that you will not be using any spawning mechanism that uses fork, you may want to put the following at the end of your Rprofile.site.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Make absolutely sure that it is after any lines that are used to load RevoScaleR:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The following are possible cases where fork may be called.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Obviously, this is not an all-inclusive list:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`nohup`</ph> to launch jobs.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This will cause a fork to be called.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Using <ph id="ph1">`multicore`</ph> and/or <ph id="ph2">`doMC`</ph> to launch R processes with RevoScaleR</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Note that when using <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept>, the default behavior for any worker node process on a Linux host will be to have the thread pool off (set to create threads in an ad hoc manner).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If the function passed to <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept> is going to make multiple calls into RevoScaleR functions, you will probably want to include a call to <ph id="ph1">`rxSetEnableThreadPool(TRUE)`</ph> as the first line of the function that you pass to <bpt id="p2">[</bpt>rxExec<ept id="p2">](rxExec.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For distributed HPA functions run on worker nodes, threading is always automatically handled for the user.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxGetEnableThreadPool`</ph> function can be used to determine whether the thread pool is instantiated or not.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Note that on Windows, it will always be instantiated; on Linux, whether it is always instantiated or created on an ad hoc basis is controlled by <ph id="ph1">`rxSetEnableThreadPool`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>At startup on Linux, the thread pool state wil be off; that is, threads will be created on an ad hoc basis.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxSetEnableThreadPool`</ph> returns the state of the thread pool prior to making the call (as opposed to the updated state).</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Thus, this function returns <ph id="ph1">`TRUE`</ph> if the thread pool was instantiated and in a ready state prior to making the call, or <ph id="ph2">`FALSE`</ph> if the thread pool was set to be created in an ad hoc fashion.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept></source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>