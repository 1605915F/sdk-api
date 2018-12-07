---
UID: NF:clusapi.OnlineClusterResource
title: OnlineClusterResource function
author: windows-sdk-content
description: Brings an offline or failed resource online.
old-location: mscs\onlineclusterresource.htm
tech.root: mscs
ms.assetid: 8ea8d741-f6f7-48eb-9678-bbb53f76a9ec
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OnlineClusterResource, OnlineClusterResource function [Failover Cluster], PCLUSAPI_ONLINE_CLUSTER_RESOURCE, PCLUSAPI_ONLINE_CLUSTER_RESOURCE function [Failover Cluster], _wolf_onlineclusterresource, clusapi/OnlineClusterResource, clusapi/PCLUSAPI_ONLINE_CLUSTER_RESOURCE, mscs.onlineclusterresource
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
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-0.dll
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-1.dll
 - Ext-MS-Win-Cluster-ClusAPI-l1-1-2.dll
api_name:
 - OnlineClusterResource
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# OnlineClusterResource function


## -description


Brings an offline or failed  <a href="https://msdn.microsoft.com/en-us/library/Aa372152(v=VS.85).aspx">resource</a> online. The <b>PCLUSAPI_ONLINE_CLUSTER_RESOURCE</b> type defines a pointer to this function.


## -parameters




### -param hResource [in]

Handle to the resource to be brought online.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://msdn.microsoft.com/en-us/library/ms681381(v=VS.85).aspx">system error code</a>. The following is a possible error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_IO_PENDING</b></dt>
</dl>
</td>
<td width="60%">
The resource or one of the resources it depends on has returned <b>ERROR_IO_PENDING</b> from its  <a href="https://msdn.microsoft.com/en-us/library/Aa371770(v=VS.85).aspx">Online</a> entry point function.

</td>
</tr>
</table>
 




## -remarks



Do not call  <b>OnlineClusterResource</b> from a resource DLL. For more information, see  <a href="https://msdn.microsoft.com/en-us/library/Aa369588(v=VS.85).aspx">Function Calls to Avoid in Resource DLLs</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa371767(v=VS.85).aspx">Offline</a>



<a href="https://msdn.microsoft.com/694dbf3d-3355-44d9-8af0-ea2baae832fd">OfflineClusterResource</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa371770(v=VS.85).aspx">Online</a>



<a href="https://msdn.microsoft.com/c699cb00-b999-45b8-b9db-570150e1a65e">OpenClusterResource</a>
 

 

