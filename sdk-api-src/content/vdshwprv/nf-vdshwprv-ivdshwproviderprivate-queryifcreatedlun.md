---
UID: NF:vdshwprv.IVdsHwProviderPrivate.QueryIfCreatedLun
title: IVdsHwProviderPrivate::QueryIfCreatedLun
author: windows-sdk-content
description: Enables VDS to determine whether the hardware provider manages the specified LUN.
old-location: base\ivdshwproviderprivate_queryifcreatedlun.htm
tech.root: VDS
ms.assetid: 06ba3486-9381-4898-b639-3d94b83be857
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsHwProviderPrivate interface [VDS],QueryIfCreatedLun method, IVdsHwProviderPrivate.QueryIfCreatedLun, IVdsHwProviderPrivate::QueryIfCreatedLun, QueryIfCreatedLun, QueryIfCreatedLun method [VDS], QueryIfCreatedLun method [VDS],IVdsHwProviderPrivate interface, base.ivdshwproviderprivate_queryifcreatedlun, vdshwprv/IVdsHwProviderPrivate::QueryIfCreatedLun
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
 - IVdsHwProviderPrivate.QueryIfCreatedLun
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsHwProviderPrivate::QueryIfCreatedLun


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Enables VDS to determine whether the hardware provider manages the specified LUN.


## -parameters




### -param pwszDevicePath [in]

A pointer to the path to the LUN on the local computer; a zero-terminated, human-readable string.


### -param pVdsLunInformation [in]

A pointer to the identification data of the specified LUN. See the <a href="https://msdn.microsoft.com/6ad7ec27-add1-4f1e-aa01-6f43c75b7ad9">VDS_LUN_INFORMATION</a>structure.


### -param pLunId [out]

A pointer to the returned LUN GUID. If the provider does not manage the LUN, set this parameter to GUID_NULL.


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
The provider owns the LUN; returns the GUID of the LUN.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The provider does not own the LUN.

</td>
</tr>
</table>
 




## -remarks



Only VDS calls this method.




## -see-also




<a href="https://msdn.microsoft.com/7e6dbf9e-9060-46bf-be11-9d9d640a3d36">IVdsHwProviderPrivate</a>



<a href="https://msdn.microsoft.com/6ad7ec27-add1-4f1e-aa01-6f43c75b7ad9">VDS_LUN_INFORMATION</a>
 

 

