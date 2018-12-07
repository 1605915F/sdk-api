---
UID: NF:clusapi.GetClusterNetInterfaceKey
title: GetClusterNetInterfaceKey function
author: windows-sdk-content
description: Opens the root of the cluster database subtree for a network interface object.
old-location: mscs\getclusternetinterfacekey.htm
tech.root: mscs
ms.assetid: c6ba405a-e485-49fc-81f4-dd6c7b7bef04
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetClusterNetInterfaceKey, GetClusterNetInterfaceKey function [Failover Cluster], _wolf_getclusternetinterfacekey, clusapi/GetClusterNetInterfaceKey, mscs.getclusternetinterfacekey
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
 - GetClusterNetInterfaceKey
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetClusterNetInterfaceKey function


## -description


Opens the root of the  <a href="https://msdn.microsoft.com/en-us/library/Aa369094(v=VS.85).aspx">cluster database</a> subtree for a  <a href="https://msdn.microsoft.com/en-us/library/Aa371519(v=VS.85).aspx">network interface</a> object.


## -parameters




### -param hNetInterface [in]

Handle to a network interface.


### -param samDesired [in]

Access mask that describes the security access needed for the key.


## -returns



If the operation succeeds, the function returns a registry key handle for the network interface.

If the operation fails, 
the function returns <b>NULL</b>. For more information about the error, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The  <b>GetClusterNetInterfaceKey</b> function returns a handle to a cluster database key representing the subtree root for the network interface identified by <i>hNetInterface</i>. Callers should call  <a href="https://msdn.microsoft.com/en-us/library/Aa368989(v=VS.85).aspx">ClusterRegCloseKey</a> to close the key handle retrieved by  <b>GetClusterNetInterfaceKey</b> when they are done with it.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa368989(v=VS.85).aspx">ClusterRegCloseKey</a>



<a href="https://msdn.microsoft.com/1198ad57-ea47-428f-8867-061afbfc7709">OpenClusterNetInterface</a>
 

 

