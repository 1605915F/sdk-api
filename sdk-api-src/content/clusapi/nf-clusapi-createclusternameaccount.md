---
UID: NF:clusapi.CreateClusterNameAccount
title: CreateClusterNameAccount function (clusapi.h)
author: windows-sdk-content
description: Creates a cluster name resource and then uses it add a cluster to a domain, even if the machines that host the cluster aren't members of the domain.
old-location: mscs\createclusternameaccount.htm
tech.root: MsCS
ms.assetid: 82BBEE9D-C787-4935-BB5F-09438676B37A
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateClusterNameAccount, CreateClusterNameAccount function [Failover Cluster], PCLUSAPI_CREATE_CLUSTER_NAME_ACCOUNT, PCLUSAPI_CREATE_CLUSTER_NAME_ACCOUNT function [Failover Cluster], clusapi/CreateClusterNameAccount, clusapi/PCLUSAPI_CREATE_CLUSTER_NAME_ACCOUNT, mscs.createclusternameaccount
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2016
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: ClusAPI.lib
req.dll: ClusAPI.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - ClusAPI.dll
api_name:
 - CreateClusterNameAccount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CreateClusterNameAccount function


## -description


Creates a <a href="https://msdn.microsoft.com/7b5b9d3f-98ab-419b-936e-26e9e5fc022d">cluster name</a> resource and then uses it add a cluster to a domain, even if the machines that host the cluster aren't members of the domain.The <b>PCLUSAPI_CREATE_CLUSTER_NAME_ACCOUNT</b> type defines a pointer to this function.


## -parameters




### -param hCluster [in]

A handle to the cluster to add the cluster name resource to.


### -param pConfig [in]

A pointer to the <a href="https://msdn.microsoft.com/21D43B28-0B14-4A00-BDEE-B2B769BF9777">CREATE_CLUSTER_NAME_ACCOUNT</a> structure that contains the information about the <a href="https://msdn.microsoft.com/7b5b9d3f-98ab-419b-936e-26e9e5fc022d">cluster name</a> resource to create, and the domain credentials to use.


### -param pfnProgressCallback [in, optional]

A pointer to the <a href="https://msdn.microsoft.com/fb7a6991-576c-4c03-aef0-89811fbc1a0d">ClusterSetupProgressCallback</a> callback function that receives the status of updates to the cluster.


### -param pvCallbackArg [in, optional]

Callback function arguments for the <i>pfnProgressCallback</i> parameter.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>. If the operation fails, the function returns a system error code.




## -see-also




<a href="https://msdn.microsoft.com/1b3a3b23-39db-47b7-b4a8-17fc1ee45df6">Failover Cluster Management Functions</a>
 

 

