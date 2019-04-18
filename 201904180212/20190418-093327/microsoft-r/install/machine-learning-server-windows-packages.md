<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-windows-packages.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4dd467dabe0fec17423410396d782b6a25fa2c87e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">dd467dabe0fec17423410396d782b6a25fa2c87e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-windows-packages.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Add or remove R and Python on Machine Learning Server for Windows</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install or uninstall R and Python packages on Machine Learning Server for Windows.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to add or remove R and Python packages on Machine Learning Server for Windows</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server 9.2.1 | 9.3<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>You can add open-source and third-party R and Python packages to the same local repository containing the product-specific packages for Machine Learning Server, allowing you to call functions from any library in the same script.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Any packages you add to the repository must be compatible with the base R and Anaconda distributions upon which Microsoft's R and Python libraries are built.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Version requirements</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Product-specific packages like RevoScaleR and revoscalepy are built on base libraries of R and Python respectively.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Any new packages that you add must be compatible with the base libraries installed with the product.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Upgrading or downgrading the base R or Python libraries installed by setup is not supported.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Microsoft's proprietary packages are built on specific distributions and versions of the base libraries.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Substituting different versions of those libraries could destabilize your installation.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Base R is distributed through Microsoft R Open, as installed by Machine Learning Server or R Server.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Python is distributed though Anaconda, also installed by Machine Learning server.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Product version</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>R version</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Anaconda/Python version</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>9.3</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>3.4.3</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>4.2/3.5</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>9.2</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>3.4.1</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>4.2/3.5</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>9.1</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>3.3.3</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>not applicable</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To verify the base library versions on your system, start a command-line tool and check the version information displayed when the tool starts.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For R, start <bpt id="p1">**</bpt>R.exe<ept id="p1">**</ept> from \Program Files\Microsoft\ML Server\R_SERVER\bin\x64.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Loading the R execution environment displays base R version information, similar to this output.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>For Python, start <bpt id="p1">**</bpt>Python.exe<ept id="p1">**</ept> from \Program Files\Microsoft\ML Server\PYTHON_SERVER.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Loading the R execution environment displays base R version information, similar to this output.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Package location</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>On Windows, packages installed and used by Machine Learning Server can be found at these locations:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For R: <ph id="ph1">`C:\Program Files\Microsoft\ML Server\R_SERVER\library`</ph></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For Python: <ph id="ph1">`C:\Program Files\Microsoft\ML Server\PYTHON_SERVER\Lib\site-packages`</ph></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Add or remove R packages</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>R packages tend to have with multiple dependencies so we generally recommend using a tool like miniCran.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For more information and alternative methodologies, see <bpt id="p1">[</bpt>R package management<ept id="p1">](../operationalize/configure-manage-r-packages.md)</ept>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Add or remove Python packages</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Run the following commands from an administrator prompt.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Using pip<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Using conda<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What's new in Machine Learning Server<ept id="p1">](../whats-new-in-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server to operationalize your analytics<ept id="p1">](../what-is-operationalization.md)</ept></source>
        </trans-unit></group></body></file></xliff>