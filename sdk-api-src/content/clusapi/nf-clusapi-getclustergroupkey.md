---
UID: NF:clusapi.GetClusterGroupKey
title: GetClusterGroupKey function
author: windows-sdk-content
description: Opens the root of the cluster database subtree for a group.
old-location: mscs\getclustergroupkey.htm
tech.root: mscs
ms.assetid: 86f34e31-f240-485f-a5b6-e4de922b8d97
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetClusterGroupKey, GetClusterGroupKey function [Failover Cluster], _wolf_getclustergroupkey, clusapi/GetClusterGroupKey, mscs.getclustergroupkey
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Enterprise, Windows Server 2008 Datacenter
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
 - GetClusterGroupKey
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetClusterGroupKey function


## -description


Opens the root of the  <a href="https://msdn.microsoft.com/en-us/library/Aa369094(v=VS.85).aspx">cluster database</a> subtree for a  <a href="https://msdn.microsoft.com/en-us/library/Aa369645(v=VS.85).aspx">group</a>.


## -parameters




### -param hGroup [in]

Handle to a group.


### -param samDesired [in]

Access mask that describes the security access needed for the key.


## -returns



If the operation succeeds, the function returns a database key handle for the group.

If the operation fails, 
the function returns <b>NULL</b>. For more information about the error, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The  <b>GetClusterGroupKey</b> function returns a handle to a cluster database key representing the subtree root for the group identified by <i>hGroup</i>. Callers should call  <a href="https://msdn.microsoft.com/en-us/library/Aa368989(v=VS.85).aspx">ClusterRegCloseKey</a> to close the key handle retrieved by  <b>GetClusterGroupKey</b> when they are done with it.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa368989(v=VS.85).aspx">ClusterRegCloseKey</a>



<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>



<a href="https://msdn.microsoft.com/0c7ef9d9-d32b-448e-9e07-6befb9b3e338">OpenClusterGroup</a>
 

 

