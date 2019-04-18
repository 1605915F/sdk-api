---
UID: NF:rpcdce.RpcObjectInqType
title: RpcObjectInqType function (rpcdce.h)
author: windows-sdk-content
description: The RpcObjectInqType function returns the type of an object.
old-location: rpc\rpcobjectinqtype.htm
tech.root: Rpc
ms.assetid: 9146d4be-4a8a-4655-bd5b-e12f81fd4d23
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: RpcObjectInqType, RpcObjectInqType function [RPC], _rpc_rpcobjectinqtype, rpc.rpcobjectinqtype, rpcdce/RpcObjectInqType
ms.topic: function
req.header: rpcdce.h
req.include-header: Rpc.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Rpcrt4.lib
req.dll: Rpcrt4.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Rpcrt4.dll
api_name:
 - RpcObjectInqType
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# RpcObjectInqType function


## -description


The 
<b>RpcObjectInqType</b> function returns the type of an object.


## -parameters




### -param ObjUuid

Pointer to the object UUID whose associated type UUID is returned.


### -param TypeUuid

Returns a pointer to the type UUID of the <i>ObjUuid</i> parameter. 




Specify a parameter value of <b>NULL</b> to prevent the return of a type UUID. In this way, an application can determine (from the returned status) whether <i>ObjUuid</i> is registered without specifying an output type UUID variable.


## -returns



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_S_OK</b></dt>
</dl>
</td>
<td width="60%">
The call succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_S_OBJECT_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
Object not found.

</td>
</tr>
</table>
 

<div class="alert"><b>Note</b>  For a list of valid error codes, see 
<a href="https://msdn.microsoft.com/0223aa7a-b0cf-49e3-9f08-90be5ccffbd1">RPC Return Values</a>.</div>
<div> </div>



## -remarks



A server application calls 
<b>RpcObjectInqType</b> to obtain the type UUID of an object. If the object was registered with the RPC run-time library using the 
<a href="https://msdn.microsoft.com/2fb22b97-97ce-403a-bfcb-101bb63f906f">RpcObjectSetType</a> function, the registered type is returned.

Optionally, an application can privately maintain an object/type registration. In this case, if the application has provided an object inquiry function (see under 
<a href="https://msdn.microsoft.com/358d3ab3-df16-486b-aeac-56a0ffc78272">RpcObjectSetInqFn</a>). The RPC run-time library uses that function to determine an object's type.

The 
<b>RpcObjectInqType</b> function obtains the type UUID as described in the following table.

<table>
<tr>
<th>Object UUID<div> </div>registered</th>
<th>Inquiry function<div> </div>registered</th>
<th>Return<div> </div>value</th>
</tr>
<tr>
<td>Yes (
<a href="https://msdn.microsoft.com/2fb22b97-97ce-403a-bfcb-101bb63f906f">RpcObjectSetType</a>)</td>
<td>Ignored</td>
<td>The object's registered type UUID.</td>
</tr>
<tr>
<td>No</td>
<td>Yes (
<a href="https://msdn.microsoft.com/358d3ab3-df16-486b-aeac-56a0ffc78272">RpcObjectSetInqFn</a>)</td>
<td>The type UUID returned from the inquiry function.</td>
</tr>
<tr>
<td>No</td>
<td>No</td>
<td>The nil UUID.</td>
</tr>
</table>
 


<div> </div>





## -see-also




<a href="https://msdn.microsoft.com/358d3ab3-df16-486b-aeac-56a0ffc78272">RpcObjectSetInqFn</a>



<a href="https://msdn.microsoft.com/2fb22b97-97ce-403a-bfcb-101bb63f906f">RpcObjectSetType</a>
 

 

