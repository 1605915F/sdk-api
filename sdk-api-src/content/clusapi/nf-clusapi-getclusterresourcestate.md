---
UID: NF:clusapi.GetClusterResourceState
title: GetClusterResourceState function
author: windows-sdk-content
description: Returns the current state of a resource.
old-location: mscs\getclusterresourcestate.htm
tech.root: MsCS
ms.assetid: c3897c96-743e-4753-8fef-b8defe4f2b00
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetClusterResourceState, GetClusterResourceState function [Failover Cluster], PCLUSAPI_GET_CLUSTER_RESOURCE_STATE, PCLUSAPI_GET_CLUSTER_RESOURCE_STATE function [Failover Cluster], _wolf_getclusterresourcestate, clusapi/GetClusterResourceState, clusapi/PCLUSAPI_GET_CLUSTER_RESOURCE_STATE, mscs.getclusterresourcestate
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
 - GetClusterResourceState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetClusterResourceState function


## -description


Returns 
    the current state of a <a href="https://msdn.microsoft.com/090d1c20-fab3-43dd-bfe2-a2c3f9ba8f89">resource</a>. The <b>PCLUSAPI_GET_CLUSTER_RESOURCE_STATE</b> type defines a pointer to this function.


## -parameters




### -param hResource [in]

Handle specifying the resource for which state information should be returned.


### -param lpszNodeName [out, optional]

Pointer to a buffer that receives the name of the specified resource's current owner node as a 
       <b>NULL</b>-terminated Unicode string. Pass <b>NULL</b> if the node name 
       is not required.


### -param lpcchNodeName [in, out, optional]

Pointer to the size of the <i>lpszNodeName</i> buffer as a count of characters. This 
       pointer cannot be <b>NULL</b> unless <i>lpszNodeName</i> is also 
       <b>NULL</b>. On input, specifies the maximum number of characters the buffer can hold, 
       including the terminating <b>NULL</b>. On output, specifies the number of characters in the 
       resulting name, excluding the terminating <b>NULL</b>.


### -param lpszGroupName [out, optional]

Pointer to a buffer that receives the name of the <a href="https://msdn.microsoft.com/1e0680ba-87d0-4bf0-808c-d80485e4daa3">group</a> that 
       contains the specified resource. The name is returned as a <b>NULL</b>-terminated Unicode 
       string. Pass <b>NULL</b> if the group name is not required.


### -param lpcchGroupName [in, out, optional]

Pointer to the size of the <i>lpszGroupName</i> buffer as a count of characters. This 
       pointer cannot be <b>NULL</b> unless <i>lpszNodeName</i> is also 
       <b>NULL</b>. On input, specifies the maximum number of characters the buffer can hold, 
       including the terminating <b>NULL</b>. On output, specifies the number of characters in the 
       resulting name, excluding the terminating <b>NULL</b>.


## -returns



<b>GetClusterResourceState</b> returns the 
       current state of the resource enumerated from the 
       <a href="https://msdn.microsoft.com/bd5dee18-a06f-4e46-a27e-c907b1c25a68">CLUSTER_RESOURCE_STATE</a> enumeration, which can be 
       represented by one of the following values.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourceInitializing</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
The resource is performing initialization.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourceOnline</b></dt>
<dt>2</dt>
</dl>
</td>
<td width="60%">
The resource is operational and functioning normally.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourceOffline</b></dt>
<dt>3</dt>
</dl>
</td>
<td width="60%">
The resource is not operational. This value will be returned if the resource reported a state of 
         <b>ClusterResourceOffline</b> (3) or 
         <b>ClusterResourceCannotComeOnlineOnThisNode</b> (127).

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourceFailed</b></dt>
<dt>4</dt>
</dl>
</td>
<td width="60%">
The resource has failed. This value will be returned if the resource reported a state of 
         <b>ClusterResourceFailed</b> (4) or 
         <b>ClusterResourceCannotComeOnlineOnAnyNode</b> (126).

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourcePending</b></dt>
<dt>128</dt>
</dl>
</td>
<td width="60%">
The resource is in the process of coming online or going offline.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourceOnlinePending</b></dt>
<dt>129</dt>
</dl>
</td>
<td width="60%">
The resource is in the process of coming online.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourceOfflinePending</b></dt>
<dt>130</dt>
</dl>
</td>
<td width="60%">
The resource is in the process of going offline.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ClusterResourceStateUnknown</b></dt>
<dt>-1</dt>
</dl>
</td>
<td width="60%">
The operation was not successful. For more information about the error, call the function 
         <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.

</td>
</tr>
</table>
 




## -remarks



Do not call <b>GetClusterResourceState</b> from 
     any resource DLL entry point function. 
     <b>GetClusterResourceState</b> can safely be called 
     from a worker thread. For more information, see 
     <a href="https://msdn.microsoft.com/0eaa4aea-8d9a-4552-b43a-fafa23a3e736">Function Calls to Avoid in Resource DLLs</a>.


#### Examples

See <a href="https://msdn.microsoft.com/de1d4ad2-3531-467e-a2e6-24d22514ce6e">Getting Object States</a> for an example.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/bd5dee18-a06f-4e46-a27e-c907b1c25a68">CLUSTER_RESOURCE_STATE</a>



<a href="https://msdn.microsoft.com/1d67a4f5-66f8-4818-8b63-d0f50452f889">Offline</a>



<a href="https://msdn.microsoft.com/694dbf3d-3355-44d9-8af0-ea2baae832fd">OfflineClusterResource</a>



<a href="https://msdn.microsoft.com/b406ef44-0622-4625-a6cf-462b6ea6018d">Online</a>



<a href="https://msdn.microsoft.com/8ea8d741-f6f7-48eb-9678-bbb53f76a9ec">OnlineClusterResource</a>



<a href="https://msdn.microsoft.com/c699cb00-b999-45b8-b9db-570150e1a65e">OpenClusterResource</a>
 

 

