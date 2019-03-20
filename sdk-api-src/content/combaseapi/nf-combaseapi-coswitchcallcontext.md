---
UID: NF:combaseapi.CoSwitchCallContext
title: CoSwitchCallContext function (combaseapi.h)
author: windows-sdk-content
description: Switches the call context object used by CoGetCallContext.
old-location: com\coswitchcallcontext.htm
tech.root: com
ms.assetid: 146855a2-97ec-4e71-88dc-316eaa1a24a0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CoSwitchCallContext, CoSwitchCallContext function [COM], _com_CoSwitchCallContext, com.coswitchcallcontext, combaseapi/CoSwitchCallContext
ms.topic: function
req.header: combaseapi.h
req.include-header: Objbase.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Ole32.lib
req.dll: Ole32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Ole32.dll
 - API-MS-Win-Core-Com-l1-1-0.dll
 - ComBase.dll
 - API-MS-Win-Core-Com-l1-1-1.dll
 - API-MS-Win-DownLevel-Ole32-l1-1-1.dll
api_name:
 - CoSwitchCallContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CoSwitchCallContext function


## -description


Switches the call context object used by <a href="https://msdn.microsoft.com/b82e32c0-840d-402e-90d5-ff678c51faf1">CoGetCallContext</a>.


## -parameters




### -param pNewObject [in, optional]

A pointer to an interface on the new call context object. COM stores this pointer without adding a reference to the pointer until <b>CoSwitchCallContext</b> is called with another object. This parameter may be <b>NULL</b> if you are calling <b>CoSwitchCallContext</b> to switch back to the original call context but there was no original call context.


### -param ppOldObject [out]

The address of pointer variable that receives a pointer to the call context object of the call currently in progress. This value is returned so that the original call context can be restored by the custom marshaller. The returned pointer will be <b>NULL</b> if there was no call in progress.


## -returns



This function can return the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The function was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUT_OF_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
Out of memory.

</td>
</tr>
</table>
 




## -remarks



Custom marshallers call <b>CoSwitchCallContext</b> to change the call context object used by the <a href="https://msdn.microsoft.com/b82e32c0-840d-402e-90d5-ff678c51faf1">CoGetCallContext</a> function. Before dispatching an arriving call, custom marshallers call <b>CoSwitchCallContext</b>, specifying the new context object. After sending a reply, they must restore the original call context by calling <b>CoSwitchCallContext</b> again, this time passing a pointer to the original context object.

<b>CoSwitchCallContext</b> does not add a reference to the new context object. Custom marshallers must ensure that the lifetime of their context object continues throughout their call and until the call to restore the original context.  Custom marshallers should not release the value that they placed into the <i>ppOldObject</i> parameter when they set their context.

Call context objects provided by custom marshallers should support the <a href="https://msdn.microsoft.com/aacef77c-7185-44ed-aa1a-465c6100a431">IServerSecurity</a> interface.





## -see-also




<a href="https://msdn.microsoft.com/b82e32c0-840d-402e-90d5-ff678c51faf1">CoGetCallContext</a>



<a href="https://msdn.microsoft.com/aacef77c-7185-44ed-aa1a-465c6100a431">IServerSecurity</a>



<a href="https://msdn.microsoft.com/c9f6d06c-da24-48ea-908a-2462c33f7ee3">Security in COM</a>
 

 

