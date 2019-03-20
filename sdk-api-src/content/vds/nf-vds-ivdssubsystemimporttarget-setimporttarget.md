---
UID: NF:vds.IVdsSubSystemImportTarget.SetImportTarget
title: IVdsSubSystemImportTarget::SetImportTarget (vds.h)
author: windows-sdk-content
description: Sets the Volume Shadow Copy service (VSS) import target for the computer for this subsystem.
old-location: base\ivdssubsystemimporttarget_setimporttarget.htm
tech.root: VDS
ms.assetid: 96770760-a9af-46be-8e63-be8a86ec81ab
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsSubSystemImportTarget interface [VDS],SetImportTarget method, IVdsSubSystemImportTarget.SetImportTarget, IVdsSubSystemImportTarget::SetImportTarget, SetImportTarget, SetImportTarget method [VDS], SetImportTarget method [VDS],IVdsSubSystemImportTarget interface, base.ivdssubsystemimporttarget_setimporttarget, vds/IVdsSubSystemImportTarget::SetImportTarget
ms.topic: method
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
 - IVdsSubSystemImportTarget.SetImportTarget
product: Windows
targetos: Windows
req.typenames: 
req.redist: VDS 1.1
---

# IVdsSubSystemImportTarget::SetImportTarget


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Sets the Volume Shadow Copy service (VSS) import target for the computer for this subsystem. Whenever shadow copies 
   are created and a LUN from a shadow copy set from the subsystem is imported onto this computer, it will be associated 
   with the import target by the VSS hardware provider.


## -parameters




### -param pwszIscsiName [in]

The <b>VDS_OBJECT_ID</b> of the target to set as the import target. Use 
      <b>GUID_NULL</b> to clear the current import target for this subsystem.


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
<dt><b><b>S_OK</b></b></dt>
</dl>
</td>
<td width="60%">
The import target was set successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_PROVIDER_CACHE_CORRUPT</b></b></dt>
<dt>0x8004241FL</dt>
</dl>
</td>
<td width="60%">
The cache of the provider is corrupted. This indicates a software or communication problem inside a 
        provider that caches information about the attached devices. The caller can use the 
        <a href="https://msdn.microsoft.com/aeb06a98-8896-446f-abd5-ea40be0bea40">IVdsHwProvider::Reenumerate</a> method 
        followed by the  <a href="https://msdn.microsoft.com/25ddc73c-5d1b-4bec-bbc2-9f22a5f82ffe">IVdsHwProvider::Refresh</a> 
        method to restore the cache.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_OBJECT_DELETED</b></b></dt>
<dt>0x8004240BL</dt>
</dl>
</td>
<td width="60%">
The subsystem object is no longer present.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_NOT_SUPPORTED</b></b></dt>
<dt>0x80042400L</dt>
</dl>
</td>
<td width="60%">
The operation or combination of parameters is not supported by this provider.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/1fff1400-61d9-494f-857d-53626b80c2d2">GetImportTarget</a>



<a href="https://msdn.microsoft.com/c9e2f353-d5d4-47a2-8398-5cbd9d499fb7">IVdsSubSystemImportTarget</a>
 

 

