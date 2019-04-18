---
title: 'Configure Jupyter Notebooks in Machine Learning Server '
description: How to configure a Jupyter notebook to call Python functions from revoscalepay and microsofml modules in Machine learning Server.
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 12/17/2018
ms.topic: conceptual
ms.prod: mlserver
ms.technology: ''
ms.openlocfilehash: 3a84c747cb15a201084639f2207314a4ec079de6
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="how-to-add-machine-learning-server-modules-to-multi-user-jupyter-notebook-instances"></a>How to add Machine Learning Server modules to multi-user Jupyter Notebook instances

This article explains how to add our libraries to a remote Jupyter server acting as central hub for multi-user notebooks on your network.

Jupyter Notebooks is distributed with Anaconda, which is the Python distribution used by Machine Learning Server. If you installed Machine Learning Server, you have the components necessary for running notebooks as a single user on localhost.

Both Machine Learning Server and Jupyter Notebooks must be on the same computer.


## <a name="configure-for-multi-user-access-on-linux"></a>Configure for multi-user access on Linux

This procedure applies to Linux or Spark edge node upon which you are hosting a JupyterHub or multi-user server. It does not apply to single-user localhost servers. 

For a multi-user server, add our custom kernel **MLSPython** to the data directory of your server. Machine Learning Server provides this kernel for notebooks and scripts that make calls to [revoscalepy](../python-reference/revoscalepy/revoscalepy-package.md), [microsoftml](../python-reference/microsoftml/microsoftml-package.md), and [azureml](../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md).

Run the following command to install the kernel:

```
sudo /usr/bin/anaconda/bin/jupyter kernelspec install /opt/microsoft/mlserver/9.2.1/libraries/jupyter/kernels/MMLSPy
```

If the `/usr/bin/anaconda/bin/jupyter` folder doesn't exist, then the server is not a JupyterHub or multi-user server. For more information, see [JupyterHub documentation](https://jupyterhub.readthedocs.io/en/stable/). 

## <a name="check-kernel-installation"></a>Check kernel installation

Verify the file is in the expected location.

1. Run `jupyter –-data-dir` from the node on which Jupyter Notebook Server is installed.
2. Note the path returned by `--data-dir`. This is where Jupyter stores its data directories, including kernels.
3. Navigate to the folder. You should see **MLSPython** listed.

If the installation command did not succeed, you can manually copy the **MLSPython** directory from `/opt/microsoft/mlserver/9.3.0/libraries/kernels/` to the kernels subdirectory under the data directory.

You might need to restart your server in order for the server to pick up the kernel.

## <a name="use-the-mmlspy-notebook-option"></a>Use the MMLSPy notebook option

In Jupyter dashboard, click **New** to create a new notebook. You should see the new kernel (MMLSPy) in the drop down.

![mmlspy kernel in New notebook list](./media/jupyternb-new-mmlspy.png)


## <a name="see-also"></a>See also

+ [microsoftml function reference](../python-reference/microsoftml/microsoftml-package.md)
+ [revoscalepy function reference](../python-reference/revoscalepy/revoscalepy-package.md)
+ [Jupyter/IPython Notebook Quick Start Guide](https://jupyter-notebook-beginner-guide.readthedocs.io)
