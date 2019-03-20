---
UID: NF:msctf.IEnumTfPropertyValue.Clone
title: IEnumTfPropertyValue::Clone (msctf.h)
author: windows-sdk-content
description: IEnumTfPropertyValue::Clone method
old-location: tsf\ienumtfpropertyvalue_clone.htm
tech.root: TSF
ms.assetid: 10c21ea3-a984-4dde-afb4-715a5273fd03
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Clone, Clone method [Text Services Framework], Clone method [Text Services Framework],IEnumTfPropertyValue interface, IEnumTfPropertyValue interface [Text Services Framework],Clone method, IEnumTfPropertyValue.Clone, IEnumTfPropertyValue::Clone, _tsf_ienumtfpropertyvalue_clone_ref, msctf/IEnumTfPropertyValue::Clone, tsf.ienumtfpropertyvalue_clone
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
 - IEnumTfPropertyValue.Clone
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# IEnumTfPropertyValue::Clone


## -description




## -parameters




### -param ppEnum [out]

Pointer to an <a href="https://msdn.microsoft.com/7f99df15-777c-46eb-bff3-542eb1fcc428">IEnumTfPropertyValue</a> interface pointer that receives the new enumerator.


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
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
The method is not implemented.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/7f99df15-777c-46eb-bff3-542eb1fcc428">IEnumTfPropertyValue
      </a>
 

 

