---
UID: NF:vds.IVdsService.QueryFileSystemTypes
title: IVdsService::QueryFileSystemTypes
author: windows-sdk-content
description: Returns property details for all file systems known to VDS.
old-location: base\ivdsservice_queryfilesystemtypes.htm
tech.root: VDS
ms.assetid: 17dcafc8-8faf-4dc2-af24-7e1ab257201e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsService interface [VDS],QueryFileSystemTypes method, IVdsService.QueryFileSystemTypes, IVdsService::QueryFileSystemTypes, QueryFileSystemTypes, QueryFileSystemTypes method [VDS], QueryFileSystemTypes method [VDS],IVdsService interface, base.ivdsservice_queryfilesystemtypes, vds/IVdsService::QueryFileSystemTypes
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
 - IVdsService.QueryFileSystemTypes
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsService::QueryFileSystemTypes


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Returns property details for all file systems known to VDS.


## -parameters




### -param ppFileSystemTypeProps [out]

The address of a pointer to a buffer holding an array of 
      <a href="https://msdn.microsoft.com/92383a59-d7dd-419b-b6d0-959fef41ad4e">VDS_FILE_SYSTEM_TYPE_PROP</a> structures. 
      Callers must free the memory for the array and for the <b>pwszIllegalLabelCharSet</b> string 
      by using the <a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a> function.


### -param plNumberOfFileSystems [out]

The total number of file systems.


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
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method completed successfully.

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
VDS failed to initialize. If an application calls this method before the service finishes initializing, 
        the method is blocked until the initialization completes. If the initialization fails, this error is 
        returned.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/6b081cc8-fe06-427f-b06d-831a1f1fef52">IVdsService</a>



<a href="https://msdn.microsoft.com/92383a59-d7dd-419b-b6d0-959fef41ad4e">VDS_FILE_SYSTEM_TYPE_PROP</a>
 

 

