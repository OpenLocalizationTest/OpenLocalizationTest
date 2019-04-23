<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscalepy-jupyter-nb-config.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca863a84c747cb15a201084639f2207314a4ec079de6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3a84c747cb15a201084639f2207314a4ec079de6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python\how-to-revoscalepy-jupyter-nb-config.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure Jupyter Notebooks in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to configure a Jupyter notebook to call Python functions from revoscalepay and microsofml modules in Machine learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to add Machine Learning Server modules to multi-user Jupyter Notebook instances</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article explains how to add our libraries to a remote Jupyter server acting as central hub for multi-user notebooks on your network.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Jupyter Notebooks is distributed with Anaconda, which is the Python distribution used by Machine Learning Server.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>If you installed Machine Learning Server, you have the components necessary for running notebooks as a single user on localhost.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Both Machine Learning Server and Jupyter Notebooks must be on the same computer.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Configure for multi-user access on Linux</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This procedure applies to Linux or Spark edge node upon which you are hosting a JupyterHub or multi-user server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>It does not apply to single-user localhost servers.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For a multi-user server, add our custom kernel <bpt id="p1">**</bpt>MLSPython<ept id="p1">**</ept> to the data directory of your server.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Machine Learning Server provides this kernel for notebooks and scripts that make calls to <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept>, <bpt id="p2">[</bpt>microsoftml<ept id="p2">](../python-reference/microsoftml/microsoftml-package.md)</ept>, and <bpt id="p3">[</bpt>azureml<ept id="p3">](../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Run the following command to install the kernel:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`/usr/bin/anaconda/bin/jupyter`</ph> folder doesn't exist, then the server is not a JupyterHub or multi-user server.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>JupyterHub documentation<ept id="p1">](https://jupyterhub.readthedocs.io/en/stable/)</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Check kernel installation</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Verify the file is in the expected location.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Run <ph id="ph1">`jupyter –-data-dir`</ph> from the node on which Jupyter Notebook Server is installed.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Note the path returned by <ph id="ph1">`--data-dir`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This is where Jupyter stores its data directories, including kernels.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Navigate to the folder.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>You should see <bpt id="p1">**</bpt>MLSPython<ept id="p1">**</ept> listed.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If the installation command did not succeed, you can manually copy the <bpt id="p1">**</bpt>MLSPython<ept id="p1">**</ept> directory from <ph id="ph1">`/opt/microsoft/mlserver/9.3.0/libraries/kernels/`</ph> to the kernels subdirectory under the data directory.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>You might need to restart your server in order for the server to pick up the kernel.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Use the MMLSPy notebook option</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In Jupyter dashboard, click <bpt id="p1">**</bpt>New<ept id="p1">**</ept> to create a new notebook.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>You should see the new kernel (MMLSPy) in the drop down.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>mmlspy kernel in New notebook list</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>microsoftml function reference</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>revoscalepy function reference</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Jupyter/IPython Notebook Quick Start Guide</source>
        </trans-unit></group></body></file></xliff>