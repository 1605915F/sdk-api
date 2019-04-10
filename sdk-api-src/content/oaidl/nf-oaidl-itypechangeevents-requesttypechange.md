---
UID: NF:oaidl.ITypeChangeEvents.RequestTypeChange
title: ITypeChangeEvents::RequestTypeChange (oaidl.h)
author: windows-sdk-content
description: Raised when a request has been made to change a type. The change can be disallowed.
old-location: automat\itypechangeevents_requesttypechange.htm
tech.root: automat
ms.assetid: 5f968395-263f-41fc-ab75-dbcc34dd50a0
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CHANGEKIND_ADDMEMBER, CHANGEKIND_CHANGEFAILED, CHANGEKIND_DELETEMEMBER, CHANGEKIND_GENERAL, CHANGEKIND_INVALIDATE, CHANGEKIND_SETDOCUMENTATION, CHANGEKIND_SETNAMES, ITypeChangeEvents interface [Automation],RequestTypeChange method, ITypeChangeEvents.RequestTypeChange, ITypeChangeEvents::RequestTypeChange, RequestTypeChange, RequestTypeChange method [Automation], RequestTypeChange method [Automation],ITypeChangeEvents interface, _oa96_ITypeChangeEvents_RequestTypeChange, automat.itypechangeevents_requesttypechange, oaidl/ITypeChangeEvents::RequestTypeChange
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
 - ITypeChangeEvents.RequestTypeChange
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITypeChangeEvents::RequestTypeChange


## -description


Raised when a request has been made to change a type. The change can be disallowed.


## -parameters




### -param changeKind [in]

The type of change.

<a id="CHANGEKIND_ADDMEMBER"></a>
<a id="changekind_addmember"></a>


#### CHANGEKIND_ADDMEMBER

<a id="CHANGEKIND_DELETEMEMBER"></a>
<a id="changekind_deletemember"></a>


#### CHANGEKIND_DELETEMEMBER

<a id="CHANGEKIND_SETNAMES"></a>
<a id="changekind_setnames"></a>


#### CHANGEKIND_SETNAMES

<a id="CHANGEKIND_SETDOCUMENTATION"></a>
<a id="changekind_setdocumentation"></a>


#### CHANGEKIND_SETDOCUMENTATION

<a id="CHANGEKIND_GENERAL"></a>
<a id="changekind_general"></a>


#### CHANGEKIND_GENERAL

<a id="CHANGEKIND_INVALIDATE"></a>
<a id="changekind_invalidate"></a>


#### CHANGEKIND_INVALIDATE

<a id="CHANGEKIND_CHANGEFAILED"></a>
<a id="changekind_changefailed"></a>


#### CHANGEKIND_CHANGEFAILED


### -param pTInfoBefore [in]

An object that implements the <a href="https://msdn.microsoft.com/f3356463-3373-4279-bae1-953378aa2680">ITypeInfo</a>, <a href="https://msdn.microsoft.com/d3a34a13-6114-4f15-9de5-60da43fde600">ITypeInfo2</a>, <a href="https://msdn.microsoft.com/c8bbb677-2666-4900-8fb9-788742eef656">ICreateTypeInfo</a>, or <a href="https://msdn.microsoft.com/34dc6f52-6864-4edb-b22d-80eef05d4c8c">ICreateTypeInfo2</a> interface and that contains the type information before the change was made. The client subscribes to this object to receive notifications about any changes. 



### -param pStrName [in]

The name of the change. This value may be null.


### -param pfCancel [out]

False to disallow the change; otherwise, true.



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
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One or more of the arguments is not valid.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory to complete the operation.


</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/5e286a4b-b36b-40d6-9a39-d572086e5a2d">ITypeChangeEvents</a>
 

 

