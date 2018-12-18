---
UID: NF:vdshwprv.IVdsProviderPrivate.OnUnload
title: IVdsProviderPrivate::OnUnload
author: windows-sdk-content
description: Prompts the provider object to uninitialize itself.
old-location: base\ivdsproviderprivate_onunload.htm
tech.root: vds
ms.assetid: 8c4b2a0b-f056-4d3f-976c-0339c930e3cf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsProviderPrivate interface [VDS],OnUnload method, IVdsProviderPrivate.OnUnload, IVdsProviderPrivate::OnUnload, OnUnload, OnUnload method [VDS], OnUnload method [VDS],IVdsProviderPrivate interface, base.ivdsproviderprivate_onunload, vdshwprv/IVdsProviderPrivate::OnUnload
ms.topic: method
req.header: vdshwprv.h
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
 - IVdsProviderPrivate.OnUnload
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsProviderPrivate::OnUnload


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Prompts the provider object to uninitialize itself.


## -parameters




### -param bForceUnload [in]

If true, VDS attempts to forcibly unload the provider. If false, VDS makes no such attempt.


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
The provider is unloaded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The provider is unable to unload at this time. VDS tries again later.

</td>
</tr>
</table>
 




## -remarks



VDS calls this method immediately before releasing the reference to the provider object. When the reference count drops to zero, the provider unloads. If the <a href="https://msdn.microsoft.com/c5b2ac78-6a23-470c-a762-26ce6358e0b6">OnLoad</a> method fails, VDS does not call <b>OnUnload</b>.

<b>Notes to implementers:  </b>You must perform all necessary clean up, even without the call to <b>OnUnload</b>.




## -see-also




<a href="https://msdn.microsoft.com/5f1c38bf-85a7-4123-becb-e8abf3052b41">IVdsProviderPrivate</a>



<a href="https://msdn.microsoft.com/c5b2ac78-6a23-470c-a762-26ce6358e0b6">IVdsProviderPrivate::OnLoad</a>
 

 

