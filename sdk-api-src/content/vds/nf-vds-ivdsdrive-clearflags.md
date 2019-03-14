---
UID: NF:vds.IVdsDrive.ClearFlags
title: IVdsDrive::ClearFlags
author: windows-sdk-content
description: Clears the flags of a drive object.
old-location: base\ivdsdrive_clearflags.htm
tech.root: VDS
ms.assetid: 195f0c13-40d7-4fad-b589-063ec4ff4efe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClearFlags, ClearFlags method [VDS], ClearFlags method [VDS],IVdsDrive interface, IVdsDrive interface [VDS],ClearFlags method, IVdsDrive.ClearFlags, IVdsDrive::ClearFlags, base.ivdsdrive_clearflags, vds/IVdsDrive::ClearFlags, vdshwprv/IVdsDrive::ClearFlags
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
 - IVdsDrive.ClearFlags
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsDrive::ClearFlags


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Clears the flags of a drive object.


## -parameters




### -param ulFlags [in]

The flags enumerated by <a href="https://msdn.microsoft.com/50ddb9d1-32c9-4fee-bb88-498380a34c85">VDS_DRIVE_FLAG</a>. Callers can clear the <b>VDS_DRF_HOTSPARE</b> flag.


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
<dt><b>VDS_E_PROVIDER_CACHE_CORRUPT</b></dt>
<dt>0x8004241FL</dt>
</dl>
</td>
<td width="60%">
This return value signals a software or communication problem inside a provider that caches information about the array. Use the <a href="https://msdn.microsoft.com/aeb06a98-8896-446f-abd5-ea40be0bea40">IVdsHwProvider::Reenumerate</a> method followed by the <a href="https://msdn.microsoft.com/25ddc73c-5d1b-4bec-bbc2-9f22a5f82ffe">IVdsHwProvider::Refresh</a> method to restore the cache.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_OBJECT_DELETED</b></dt>
<dt>0x8004240BL</dt>
</dl>
</td>
<td width="60%">
The controller object is no longer present.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_OBJECT_STATUS_FAILED</b></dt>
<dt>0x80042431L</dt>
</dl>
</td>
<td width="60%">
The drive is in a failed state, and is unable to perform the requested operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_ANOTHER_CALL_IN_PROGRESS</b></dt>
<dt>0x80042404L</dt>
</dl>
</td>
<td width="60%">
Another operation is in progress; this operation cannot proceed until the previous operation or operations are complete.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_NOT_SUPPORTED</b></dt>
<dt>0x80042400L</dt>
</dl>
</td>
<td width="60%">
This operation or combination of parameters is not supported by this provider.

</td>
</tr>
</table>
 




## -remarks



Use <a href="https://msdn.microsoft.com/73f20f2b-44ec-44f0-b4e9-2aa40e85cc7c">IVdsDrive::SetFlags</a>to set drive flags and <a href="https://msdn.microsoft.com/31556be6-ff03-492f-a7a6-dec37a63e88d">IVdsDrive::GetProperties</a>to get currently set flags.




## -see-also




<a href="https://msdn.microsoft.com/597917cf-fb02-4949-98c3-3da3f7449ed1">IVdsDrive</a>



<a href="https://msdn.microsoft.com/31556be6-ff03-492f-a7a6-dec37a63e88d">IVdsDrive::GetProperties</a>



<a href="https://msdn.microsoft.com/73f20f2b-44ec-44f0-b4e9-2aa40e85cc7c">IVdsDrive::SetFlags</a>



<a href="https://msdn.microsoft.com/aeb06a98-8896-446f-abd5-ea40be0bea40">IVdsHwProvider::Reenumerate</a>



<a href="https://msdn.microsoft.com/25ddc73c-5d1b-4bec-bbc2-9f22a5f82ffe">IVdsHwProvider::Refresh</a>



<a href="https://msdn.microsoft.com/50ddb9d1-32c9-4fee-bb88-498380a34c85">VDS_DRIVE_FLAG</a>



<a href="https://msdn.microsoft.com/c17f13f6-ccea-4370-84d1-b422efb63e73">VDS_DRIVE_PROP</a>
 

 

