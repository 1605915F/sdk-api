---
UID: NF:vds.IVdsVolumeMF2.GetFileSystemTypeName
title: IVdsVolumeMF2::GetFileSystemTypeName
author: windows-sdk-content
description: Retrieves the name of the file system on a volume.
old-location: base\ivdsvolumemf2_getfilesystemtypename.htm
tech.root: VDS
ms.assetid: f9e8627b-0531-4dcb-9818-7560372aa4b0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetFileSystemTypeName, GetFileSystemTypeName method, GetFileSystemTypeName method,IVdsVolumeMF2 interface, IVdsVolumeMF2 interface,GetFileSystemTypeName method, IVdsVolumeMF2.GetFileSystemTypeName, IVdsVolumeMF2::GetFileSystemTypeName, base.ivdsvolumemf2_getfilesystemtypename, vds/IVdsVolumeMF2::GetFileSystemTypeName
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
 - IVdsVolumeMF2.GetFileSystemTypeName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsVolumeMF2::GetFileSystemTypeName


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Retrieves the name of the file system on a volume.


## -parameters




### -param ppwszFileSystemTypeName [out]

Pointer that upon successful completion receives a null-terminated Unicode string with the file system name.


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
 

 

