---
UID: NF:ocidl.IPerPropertyBrowsing.GetPredefinedValue
title: IPerPropertyBrowsing::GetPredefinedValue
author: windows-sdk-content
description: Retrieves the value of the specified property that is associated with a predefined string name.
old-location: com\iperpropertybrowsing_getpredefinedvalue.htm
tech.root: com
ms.assetid: a532ebed-3ed8-4b49-a17f-f542fdbd74ff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPredefinedValue, GetPredefinedValue method [COM], GetPredefinedValue method [COM],IPerPropertyBrowsing interface, IPerPropertyBrowsing interface [COM],GetPredefinedValue method, IPerPropertyBrowsing.GetPredefinedValue, IPerPropertyBrowsing::GetPredefinedValue, _ctrl_iperpropertybrowsing_getpredefinedvalue, com.iperpropertybrowsing_getpredefinedvalue, ocidl/IPerPropertyBrowsing::GetPredefinedValue
ms.topic: method
req.header: ocidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OCIdl.idl
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
 - OCIdl.h
api_name:
 - IPerPropertyBrowsing.GetPredefinedValue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPerPropertyBrowsing::GetPredefinedValue


## -description


Retrieves the value of the specified property that is associated with a predefined string name. This property is associated with a predefined string name as returned from <a href="https://msdn.microsoft.com/1b20585f-2bcd-475e-abee-80158692ae0f">IPerPropertyBrowsing::GetPredefinedStrings</a>. The predefined string is identified by a token returned from <b>GetPredefinedStrings</b>.



## -parameters




### -param dispID [in]

The dispatch identifier of the property for which a predefined value is requested.


### -param dwCookie [in]

A token identifying which value to return. The token was previously returned in the <i>pCaCookiesOut</i> array filled by <a href="https://msdn.microsoft.com/1b20585f-2bcd-475e-abee-80158692ae0f">GetPredefinedStrings</a>.


### -param pVarOut [out]

A pointer to the <b>VARIANT</b> value for the property.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, and E_UNEXPECTED, as well as the following values.

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
The method completed succesfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
This object does not support predefined strings or predefined values.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The address in <i>pVarOut</i> is not valid. For example, it may be <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



<h3><a id="Notes_to_Callers"></a><a id="notes_to_callers"></a><a id="NOTES_TO_CALLERS"></a>Notes to Callers</h3>
The caller is responsible for freeing any allocations contained in the <b>VARIANT</b>. Unless the <b>vt</b> member of <b>VARIANT</b> is VT_VARIANT, the caller can free memory using a single call to <b>VariantClear</b>. Otherwise, the caller must recursively free the contained <b>VARIANT</b> values before freeing the outer <b>VARIANT</b>.

<h3><a id="Notes_to_Implementers"></a><a id="notes_to_implementers"></a><a id="NOTES_TO_IMPLEMENTERS"></a>Notes to Implementers</h3>
Support for predefined names and values is not required. If your object does not support these names, return E_NOTIMPL from this method. If this method is not implemented, <a href="https://msdn.microsoft.com/1b20585f-2bcd-475e-abee-80158692ae0f">IPerPropertyBrowsing::GetPredefinedStrings</a> must not be implemented either.

This method allocates any memory needed inside the <b>VARIANT</b>.




## -see-also




<a href="https://msdn.microsoft.com/05e46df3-b6c8-4520-af11-21e1ff90fb9f">IPerPropertyBrowsing</a>
 

 

