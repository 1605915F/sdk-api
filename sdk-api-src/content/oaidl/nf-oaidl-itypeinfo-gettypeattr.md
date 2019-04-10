---
UID: NF:oaidl.ITypeInfo.GetTypeAttr
title: ITypeInfo::GetTypeAttr (oaidl.h)
author: windows-sdk-content
description: Retrieves a TYPEATTR structure that contains the attributes of the type description.
old-location: automat\itypeinfo_gettypeattr.htm
tech.root: automat
ms.assetid: 62be8a38-1d51-4b54-b224-7d9cdbb1be59
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetTypeAttr, GetTypeAttr method [Automation], GetTypeAttr method [Automation],ITypeInfo interface, ITypeInfo interface [Automation],GetTypeAttr method, ITypeInfo.GetTypeAttr, ITypeInfo::GetTypeAttr, _oa96_ITypeInfo_GetTypeAttr, automat.itypeinfo_gettypeattr, oaidl/ITypeInfo::GetTypeAttr
ms.topic: method
req.header: oaidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OaIdl.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - oaidl.h
api_name:
 - ITypeInfo.GetTypeAttr
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITypeInfo::GetTypeAttr


## -description


Retrieves a TYPEATTR structure that contains the attributes of the type description.


## -parameters




### -param ppTypeAttr [out]

The attributes of this type description.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK
</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG
</b></dt>
</dl>
</td>
<td width="60%">
One or more of the arguments is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY
</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory to complete the operation.

</td>
</tr>
</table>
 




## -remarks



To free the TYPEATTR structure, use <a href="https://msdn.microsoft.com/86827f7f-d5c7-4297-8eb9-af7b03d16121">ITypeInfo::ReleaseTypeAttr</a>.





## -see-also




<a href="https://msdn.microsoft.com/f3356463-3373-4279-bae1-953378aa2680">ITypeInfo</a>
 

 

