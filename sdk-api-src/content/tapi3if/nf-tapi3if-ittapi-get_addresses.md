---
UID: NF:tapi3if.ITTAPI.get_Addresses
title: ITTAPI::get_Addresses
author: windows-sdk-content
description: The get_Addresses method creates a collection of addresses that are currently available. Provided for Automation client applications, such as those written in Visual Basic. C and C++ applications must use the EnumerateAddresses method.
old-location: tapi3\ittapi_get_addresses.htm
tech.root: tapi
ms.assetid: 9e70ae94-20a2-4ba4-ab39-794f611011d8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITTAPI interface [TAPI 2.2],get_Addresses method, ITTAPI.get_Addresses, ITTAPI::get_Addresses, _tapi3_ittapi_get_addresses, get_Addresses, get_Addresses method [TAPI 2.2], get_Addresses method [TAPI 2.2],ITTAPI interface, tapi3.ittapi_get_addresses, tapi3if/ITTAPI::get_Addresses
ms.topic: method
req.header: tapi3if.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITTAPI.get_Addresses
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITTAPI::get_Addresses


## -description


The 
<b>get_Addresses</b> method creates a collection of addresses that are currently available. Provided for Automation client applications, such as those written in Visual Basic. C and C++ applications must use the 
<a href="https://msdn.microsoft.com/b40a2071-24bf-470c-bfba-de23317e8652">EnumerateAddresses</a> method.


## -parameters




### -param pVariant [out]

Pointer to a <b>VARIANT</b> containing an 
<a href="https://msdn.microsoft.com/2286678a-68b9-4f4a-b36b-7fdf8cdad6a6">ITCollection</a> of 
<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a> interface pointers (address objects).


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>pVariant</i> parameter is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>pVariant</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -remarks



TAPI calls the <b>Addref</b> method on the 
<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a> interface returned by <b>ITTAPI::get_Addesses</b>. The application must call <b>Release</b> on the 
<b>ITAddress</b> interface to free resources associated with it.




## -see-also




<a href="https://msdn.microsoft.com/b40a2071-24bf-470c-bfba-de23317e8652">EnumerateAddresses</a>



<a href="https://msdn.microsoft.com/bfe9f12e-ceb7-4120-8193-70feb2bc7c85">IEnumAddress</a>



<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a>



<a href="https://msdn.microsoft.com/2286678a-68b9-4f4a-b36b-7fdf8cdad6a6">ITCollection</a>



<a href="https://msdn.microsoft.com/75d641c7-dbf8-4ae2-b16b-2757e890d32b">ITTAPI</a>



<a href="https://msdn.microsoft.com/c4cf358f-2dc8-432a-92ed-68282ddc8a97">TAPI Object</a>
 

 

