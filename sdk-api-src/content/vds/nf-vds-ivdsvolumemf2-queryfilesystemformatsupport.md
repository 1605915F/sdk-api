---
UID: NF:vds.IVdsVolumeMF2.QueryFileSystemFormatSupport
title: IVdsVolumeMF2::QueryFileSystemFormatSupport (vds.h)
author: windows-sdk-content
description: Retrieves the properties of the file systems that are supported for formatting a volume.
old-location: base\ivdsvolumemf2_queryfilesystemformatsupport.htm
tech.root: VDS
ms.assetid: 770a92fb-9e70-4db0-a782-b9064daef4ef
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVdsVolumeMF2 interface,QueryFileSystemFormatSupport method, IVdsVolumeMF2.QueryFileSystemFormatSupport, IVdsVolumeMF2::QueryFileSystemFormatSupport, QueryFileSystemFormatSupport, QueryFileSystemFormatSupport method, QueryFileSystemFormatSupport method,IVdsVolumeMF2 interface, base.ivdsvolumemf2_queryfilesystemformatsupport, vds/IVdsVolumeMF2::QueryFileSystemFormatSupport
ms.topic: method
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - IVdsVolumeMF2.QueryFileSystemFormatSupport
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVdsVolumeMF2::QueryFileSystemFormatSupport


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Retrieves the properties of the file systems that are supported for formatting a volume.


## -parameters




### -param ppFileSystemSupportProps [out]

A pointer to the array of <a href="https://msdn.microsoft.com/0a0863d3-a97f-4be5-bba4-15d6bbbf03a5">VDS_FILE_SYSTEM_FORMAT_SUPPORT_PROP</a> structures passed in by the caller. Upon successful completion, these structures contain information about the properties of the supported file systems. Callers must free this array by using the 
      <a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a> function.


### -param plNumberOfFileSystems [out]

A pointer to a variable that upon successful completion receives the total number of elements in array pointed to by the <i>ppFileSystemSupportProps</i> parameter.


## -returns



This method can return standard HRESULT values, such as E_INVALIDARG or E_OUTOFMEMORY, and <a href="https://msdn.microsoft.com/c9ddd3b7-f017-4880-976a-c879a40dc17b">VDS-specific return values</a>. It can also return converted <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error codes</a>  using the <a href="https://msdn.microsoft.com/en-us/library/ms680746(v=VS.85).aspx">HRESULT_FROM_WIN32</a> macro. Errors can originate from VDS itself or from the underlying <a href="https://msdn.microsoft.com/b2f7628c-b567-40a9-9ad7-6c47077af5fb">VDS provider</a> that is being used. Possible return values include the following.

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
The method completed successfully.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/3219233e-7141-472a-8cb9-207222a4e775">IVdsVolumeMF2</a>
 

 

