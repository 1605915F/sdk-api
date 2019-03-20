---
UID: NF:vds.IVdsIscsiTarget.GetConnectedInitiators
title: IVdsIscsiTarget::GetConnectedInitiators (vds.h)
author: windows-sdk-content
description: Returns the list of iSCSI names of the initiators currently logged into the target.
old-location: base\ivdsiscsitarget_getconnectedinitiators.htm
tech.root: VDS
ms.assetid: 2060f012-169c-4077-a6ed-cef362f926d4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetConnectedInitiators, GetConnectedInitiators method [VDS], GetConnectedInitiators method [VDS],IVdsIscsiTarget interface, IVdsIscsiTarget interface [VDS],GetConnectedInitiators method, IVdsIscsiTarget.GetConnectedInitiators, IVdsIscsiTarget::GetConnectedInitiators, base.ivdsiscsitarget_getconnectedinitiators, vds/IVdsIscsiTarget::GetConnectedInitiators, vdshwprv/IVdsIscsiTarget::GetConnectedInitiators
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
 - IVdsIscsiTarget.GetConnectedInitiators
product: Windows
targetos: Windows
req.typenames: 
req.redist: VDS 1.1
---

# IVdsIscsiTarget::GetConnectedInitiators


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Returns the list of iSCSI names of the initiators currently logged into the 
   target.


## -parameters




### -param pppwszInitiatorList [out]

The address of a variable that receives an array of strings containing the iSCSI names of the initiators currently logged into the 
      target. Callers must free each string in this array, as well as the array itself, by using the 
      <a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a> function.


### -param plNumberOfInitiators [out]

A pointer to the number of strings returned in <i>pppwszInitiatorList</i>.


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
The list of connected initiators was returned successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>VDS_E_ANOTHER_CALL_IN_PROGRESS</b></b></dt>
<dt>0x80042404L</dt>
</dl>
</td>
<td width="60%">
Another operation is in progress; this operation cannot proceed until the previous operations are 
        complete.

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
The target object is no longer present.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/0db442c4-6cc1-43b2-8ac8-8b17cadb1101">IVdsIscsiTarget</a>
 

 

