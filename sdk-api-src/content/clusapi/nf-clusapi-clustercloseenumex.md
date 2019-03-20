---
UID: NF:clusapi.ClusterCloseEnumEx
title: ClusterCloseEnumEx function (clusapi.h)
author: windows-sdk-content
description: Closes a handle to an enumeration that was opened by the ClusterOpenEnumEx function.
old-location: mscs\clustercloseenumex.htm
tech.root: MsCS
ms.assetid: B62F1259-C4FF-45FC-9EA1-24CABFE1C0F3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClusterCloseEnumEx, ClusterCloseEnumEx function [Failover Cluster], PCLUSAPI_CLUSTER_CLOSE_ENUM_EX, PCLUSAPI_CLUSTER_CLOSE_ENUM_EX function [Failover Cluster], clusapi/ClusterCloseEnumEx, clusapi/PCLUSAPI_CLUSTER_CLOSE_ENUM_EX, mscs.clustercloseenumex
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2 Datacenter, Windows Server 2008 R2 Enterprise
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
 - ClusterCloseEnumEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterCloseEnumEx function


## -description


Closes a handle to an enumeration that was opened by the <a href="https://msdn.microsoft.com/DA35A67E-6F20-47CC-A96A-591702A79EF5">ClusterOpenEnumEx</a> function.


## -parameters




### -param hClusterEnum [in]

The handle to the cluster enumeration  to close. This is a handle that originally was returned by <a href="https://msdn.microsoft.com/DA35A67E-6F20-47CC-A96A-591702A79EF5">ClusterOpenEnumEx</a>.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>.




## -see-also




<a href="https://msdn.microsoft.com/1b3a3b23-39db-47b7-b4a8-17fc1ee45df6">Failover Cluster Management Function</a>
 

 

