---
UID: NF:msctf.ITfFunctionProvider.GetDescription
title: ITfFunctionProvider::GetDescription
author: windows-sdk-content
description: ITfFunctionProvider::GetDescription method
old-location: tsf\itffunctionprovider_getdescription.htm
tech.root: TSF
ms.assetid: a970c93f-2a1b-44b9-9177-fd69795ae9ee
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDescription, GetDescription method [Text Services Framework], GetDescription method [Text Services Framework],ITfFunctionProvider interface, ITfFunctionProvider interface [Text Services Framework],GetDescription method, ITfFunctionProvider.GetDescription, ITfFunctionProvider::GetDescription, _tsf_itffunctionprovider_getdescription_ref, msctf/ITfFunctionProvider::GetDescription, tsf.itffunctionprovider_getdescription
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: msctf.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Msctf.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Msctf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - msctf.dll
api_name:
 - ITfFunctionProvider.GetDescription
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfFunctionProvider::GetDescription


## -description




## -parameters




### -param pbstrDesc [out]

Pointer to a BSTR that receives the description string. This value must be allocated using <a href="https://msdn.microsoft.com/en-us/library/ms221458(v=VS.85).aspx">SysAllocString</a>. The caller must this memory using <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> when it is no longer required.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
A memory allocation failure occurred.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
<i>pbstrDesc</i> is invalid.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/e63fd561-1157-49b1-a981-e578d9538876">ITfFunctionProvider</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221458(v=VS.85).aspx">SysAllocString</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a>
 

 

