---
UID: NF:vdshwprv.IVdsIscsiPortalGroup.GetProperties
title: IVdsIscsiPortalGroup::GetProperties
author: windows-sdk-content
description: Returns the properties of a portal group.
old-location: base\ivdsiscsiportalgroup_getproperties.htm
tech.root: vds
ms.assetid: 7257101e-04a5-41d5-b4fa-401106610dcf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetProperties, GetProperties method [VDS], GetProperties method [VDS],IVdsIscsiPortalGroup interface, IVdsIscsiPortalGroup interface [VDS],GetProperties method, IVdsIscsiPortalGroup.GetProperties, IVdsIscsiPortalGroup::GetProperties, base.ivdsiscsiportalgroup_getproperties, vds/IVdsIscsiPortalGroup::GetProperties, vdshwprv/IVdsIscsiPortalGroup::GetProperties
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: vdshwprv.h
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
 - IVdsIscsiPortalGroup.GetProperties
product: Windows
targetos: Windows
req.typenames: 
req.redist: VDS 1.1
---

# IVdsIscsiPortalGroup::GetProperties


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Returns the properties of a portal group.


## -parameters




### -param pPortalGroupProp [out]

The address of a <a href="https://msdn.microsoft.com/82f891a2-432b-4503-8b5a-a79bea800525">VDS_ISCSI_PORTALGROUP_PROP</a> 
      structure allocated and passed in by the caller.


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
The properties were returned successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_S_PROPERTIES_INCOMPLETE</b></b></dt>
<dt>0x00042715L</dt>
</dl>
</td>
<td width="60%">
Some but not all of the properties were successfully retrieved. Note that there are many possible reasons for failing to retrieve all properties, including device removal.

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
The cache of the provider is corrupted. This indicates a software or communication problem inside a provider 
        that caches information about the attached devices. The caller can use the 
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
The portal group object is no longer present.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/65d773bd-3828-4c9d-a841-bb85a53aeadc">IVdsIscsiPortalGroup</a>



<a href="https://msdn.microsoft.com/82f891a2-432b-4503-8b5a-a79bea800525">VDS_ISCSI_PORTALGROUP_PROP</a>
 

 

