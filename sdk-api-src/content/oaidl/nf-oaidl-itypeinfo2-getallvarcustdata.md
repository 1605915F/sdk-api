---
UID: NF:oaidl.ITypeInfo2.GetAllVarCustData
title: ITypeInfo2::GetAllVarCustData
author: windows-sdk-content
description: Gets the variable for the custom data.
old-location: automat\itypeinfo2_getallvarcustdata.htm
tech.root: automat
ms.assetid: d123b63e-8393-4c76-914e-87aa399aae1c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAllVarCustData, GetAllVarCustData method [Automation], GetAllVarCustData method [Automation],ITypeInfo2 interface, ITypeInfo2 interface [Automation],GetAllVarCustData method, ITypeInfo2.GetAllVarCustData, ITypeInfo2::GetAllVarCustData, _oa96_ITypeInfo2_GetAllVarCustData, automat.itypeinfo2_getallvarcustdata, oaidl/ITypeInfo2::GetAllVarCustData
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
 - ITypeInfo2.GetAllVarCustData
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITypeInfo2::GetAllVarCustData


## -description


Gets the variable for the custom data.


## -parameters




### -param index [in]

The index of the variable for which to get the custom data.




### -param pCustData [out]

The custom data items.


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
 




## -see-also




<a href="https://msdn.microsoft.com/d3a34a13-6114-4f15-9de5-60da43fde600">ITypeInfo2</a>
 

 

