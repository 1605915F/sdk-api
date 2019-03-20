---
UID: NF:vds.IVdsService.GetObject
title: IVdsService::GetObject (vds.h)
author: windows-sdk-content
description: Returns an object pointer for the identified object.
old-location: base\ivdsservice_getobject.htm
tech.root: VDS
ms.assetid: 622a95a4-0e8c-4f65-a935-61cb48379065
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetObject, GetObject method [VDS], GetObject method [VDS],IVdsService interface, IVdsService interface [VDS],GetObject method, IVdsService.GetObject, IVdsService::GetObject, base.ivdsservice_getobject, vds/IVdsService::GetObject
ms.topic: method
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Uuid.lib
 - Uuid.dll
api_name:
 - IVdsService.GetObject
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsService::GetObject


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Returns an object pointer 
   for the identified object.


## -parameters




### -param ObjectId [in]

The GUID of the desired object.


### -param type [in]

A <a href="https://msdn.microsoft.com/63997e08-b6d3-4011-8946-56ef9832c0e4">VDS_OBJECT_TYPE</a> enumeration value that specifies the object type. 
      <b>VDS_OT_UNKNOWN</b>, <b>VDS_OT_PROVIDER</b>, 
      <b>VDS_OT_ASYNC</b>, <b>VDS_OT_ENUM</b>, and <b>VDS_OT_OPEN_VDISK</b> are not supported.
     


### -param ppObjectUnk [out]

A pointer to a buffer that receives the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> pointer to the object. When the pointer is no longer needed, the caller should release it by calling the <a href="https://msdn.microsoft.com/en-us/library/ms682317(v=VS.85).aspx">IUnknown::Release</a> method. 


## -returns



This method can return standard HRESULT values, such as E_INVALIDARG or E_OUTOFMEMORY, and <a href="https://msdn.microsoft.com/c9ddd3b7-f017-4880-976a-c879a40dc17b">VDS-specific return values</a>. It can also return converted <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error codes</a>  using the <a href="https://msdn.microsoft.com/en-us/library/ms680746(v=VS.85).aspx">HRESULT_FROM_WIN32</a> macro. Errors can originate from VDS itself or from the underlying <a href="https://msdn.microsoft.com/b2f7628c-b567-40a9-9ad7-6c47077af5fb">VDS provider</a> that is being used. Possible return values include the following.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_OBJECT_NOT_FOUND</b></dt>
<dt>0x80042405L</dt>
</dl>
</td>
<td width="60%">
An object with the specified identifier and type is not found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INITIALIZED_FAILED</b></dt>
<dt>0x80042401L</dt>
</dl>
</td>
<td width="60%">
VDS failed to initialize. If an application calls this method before the service finishes initializing, the 
        method is blocked until the initialization completes. If the initialization fails, this error is returned.

</td>
</tr>
</table>
 




## -remarks



VDS notifications return an object identifier instead of an object pointer. Callers  use this method to get a 
    pointer to the object referenced in the notification.




## -see-also




<a href="https://msdn.microsoft.com/6b081cc8-fe06-427f-b06d-831a1f1fef52">IVdsService</a>



<a href="https://msdn.microsoft.com/63997e08-b6d3-4011-8946-56ef9832c0e4">VDS_OBJECT_TYPE</a>
 

 

