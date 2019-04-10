---
UID: NF:clusapi.ClusterResourceControlAsUser
title: ClusterResourceControlAsUser function (clusapi.h)
author: windows-sdk-content
description: Initiates an operation affecting a resource.
old-location: mscs\clusterresourcecontrolasuser.htm
tech.root: MsCS
ms.assetid: D8CA1B1C-7061-4EAD-B4A0-8468B503D96D
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ClusterResourceControlAsUser, ClusterResourceControlAsUser function [Failover Cluster], clusapi/ClusterResourceControlAsUser, mscs.clusterresourcecontrolasuser
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
 - ClusterResourceControlAsUser
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterResourceControlAsUser function


## -description


Initiates an operation affecting a <a href="https://msdn.microsoft.com/090d1c20-fab3-43dd-bfe2-a2c3f9ba8f89">resource</a>.

The operation performed depends on the <a href="https://msdn.microsoft.com/47618915-0985-4415-b7d4-5959fb27eb9f">control code</a> passed 
    to the <i>dwControlCode</i> parameter.


## -parameters




### -param hResource [in]

Handle to the resource to be affected.


### -param hHostNode [in, optional]

Optional handle to the node to perform the operation. If <b>NULL</b>, the node that owns 
       the resource identified by <i>hResource</i> performs the operation.


### -param dwControlCode [in]

A <a href="https://msdn.microsoft.com/71ec60fd-67ec-4932-983b-f78c6b552954">resource control code</a>, enumerated by the 
       <a href="https://msdn.microsoft.com/c90420de-48e9-4105-9848-a27abad9c452">CLUSCTL_RESOURCE_CODES</a> enumeration, specifying 
       the operation to be performed. For the syntax associated with a control code, refer to  
       the link on the <b>CLUSCTL_RESOURCE_CODES</b> topic.


### -param lpInBuffer [in, optional]

Pointer to an input buffer containing information needed for the operation, or <b>NULL</b> 
       if no information is needed.


### -param cbInBufferSize [in]

The allocated size (in bytes) of the input buffer.


### -param lpOutBuffer [out, optional]

Pointer to an output buffer to receive the data resulting from the operation, or 
       <b>NULL</b> if no data will be returned.


### -param cbOutBufferSize [in]

The allocated size (in bytes) of the output buffer.


### -param lpBytesReturned [out, optional]

Returns the actual size (in bytes) of the data resulting from the operation. If this information is not 
       needed, pass <b>NULL</b> for <i>lpBytesReturned</i>.


## -returns



The function returns one of the following values.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The operation was successful. If the operation required an output buffer, 
         <i>lpBytesReturned</i> (if not <b>NULL</b> on input) points to the 
         actual size of the data returned in the buffer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_MORE_DATA</b></dt>
<dt>234 (0xEA)</dt>
</dl>
</td>
<td width="60%">
The output buffer pointed to by <i>lpOutBuffer</i> was not large enough to hold the data 
         resulting from the operation. The <i>lpBytesReturned</i> parameter (if not 
         <b>NULL</b> on input) points to the size required for the output buffer. Only operations 
         requiring an output buffer return <b>ERROR_MORE_DATA</b>. If the 
         <i>lpOutBuffer</i> parameter is <b>NULL</b> and the 
         <i>cbOutBufferSize</i> parameter is zero, then <b>ERROR_SUCCESS</b> may 
         be returned, not <b>ERROR_MORE_DATA</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_RESOURCE_PROPERTIES_STORED</b></dt>
<dt>5024 (0x13A0)</dt>
</dl>
</td>
<td width="60%">
Applies only to 
         <a href="https://msdn.microsoft.com/016ca8bf-b5e4-4e7e-9ffd-14120146eedd">CLUSCTL_RESOURCE_SET_COMMON_PROPERTIES</a> 
         and 
         <a href="https://msdn.microsoft.com/fdf7f7c3-fdaf-4c8e-8b57-8eab4256d5eb">CLUSCTL_RESOURCE_SET_PRIVATE_PROPERTIES</a>. 
         Indicates that the properties were successfully stored but have not yet been applied to the resource. The new 
         properties will take effect after the resource is taken offline and brought online again.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_HOST_NODE_NOT_RESOURCE_OWNER</b></dt>
<dt>5015 (0x1397)</dt>
</dl>
</td>
<td width="60%">
The node specified by the <i>hNode</i> parameter is not the node that owns the resource 
         specified by <i>hResource</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">System error code</a></b></dt>
</dl>
</td>
<td width="60%">
The operation was not successful. If the operation required an output buffer, the value specified by 
         <i>lpBytesReturned</i> (if not <b>NULL</b> on input) is 
         unreliable.

</td>
</tr>
</table>
 




## -remarks



When <a href="https://msdn.microsoft.com/a98ca55a-6535-48cf-a925-5005baa01b94">ClusterResourceControl</a> returns 
     <b>ERROR_MORE_DATA</b>, set <i>cbOutBufferSize</i> to the number of bytes 
     pointed to by <i>lpBytesReturned</i>, and call the function again.

Do not pass LPC and RPC handles to the same function call. Otherwise, the call will raise an RPC exception and 
     can have additional destructive effects. For information on how LPC and RPC handles are created, see 
     <a href="https://msdn.microsoft.com/0fdb2024-9b04-4a38-baf9-3cdabba9bf8c">LPC and RPC Handles</a> and 
     <a href="https://msdn.microsoft.com/b2ee2575-cc1e-4696-8e95-9798fb556c58">OpenCluster</a>.

The <a href="https://msdn.microsoft.com/a98ca55a-6535-48cf-a925-5005baa01b94">ClusterResourceControl</a> function is one 
     of the <a href="https://msdn.microsoft.com/89ae667e-6ad9-453e-b370-b3d6a67172a2">control code functions</a>. For more information 
     on control codes and control code functions, see 
     <a href="https://msdn.microsoft.com/20f87f60-6237-459a-93bc-f599391e65b0">Using Control Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/b2ee2575-cc1e-4696-8e95-9798fb556c58">OpenCluster</a>



<a href="https://msdn.microsoft.com/a854829d-ed05-40a0-b7c8-c3e5ab888220">Resource Type Control Codes</a>
 

 

