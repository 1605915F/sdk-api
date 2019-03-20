---
UID: NF:vds.IVdsDrive.QueryExtents
title: IVdsDrive::QueryExtents (vds.h)
author: windows-sdk-content
description: Returns an array of the extents on a drive, including both allocated and unallocated extents.
old-location: base\ivdsdrive_queryextents.htm
tech.root: VDS
ms.assetid: 8ee3e085-ce69-457e-b652-bb9c45b7fdd8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsDrive interface [VDS],QueryExtents method, IVdsDrive.QueryExtents, IVdsDrive::QueryExtents, QueryExtents, QueryExtents method [VDS], QueryExtents method [VDS],IVdsDrive interface, base.ivdsdrive_queryextents, vds/IVdsDrive::QueryExtents, vdshwprv/IVdsDrive::QueryExtents
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
 - IVdsDrive.QueryExtents
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsDrive::QueryExtents


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Returns an array of 
   the extents on a drive, including both allocated and unallocated extents.


## -parameters




### -param ppExtentArray [out]

A pointer to the  array of <a href="https://msdn.microsoft.com/c155d925-e86f-4bec-9032-dae2221172a7">VDS_DRIVE_EXTENT</a> structures passed in by the caller. Callers must free this array by using the 
      <a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a> function.


### -param plNumberOfExtents [out]

A pointer to the number of drive extents returned in the 
      <a href="https://msdn.microsoft.com/c155d925-e86f-4bec-9032-dae2221172a7">VDS_DRIVE_EXTENT</a> structure.


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
The extents information was returned successfully. For a drive without extents, the array is empty, the value 
        of <i>plNumberOfExtents</i> is set to 0, and the value of 
        <i>ppExtentArray</i> is set to <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_PROVIDER_CACHE_CORRUPT</b></dt>
<dt>0x8004241FL</dt>
</dl>
</td>
<td width="60%">
This return value signals a software or communication problem inside a provider that caches information about 
        the array. Use the 
        <a href="https://msdn.microsoft.com/aeb06a98-8896-446f-abd5-ea40be0bea40">IVdsHwProvider::Reenumerate</a> method
        followed by the <a href="https://msdn.microsoft.com/25ddc73c-5d1b-4bec-bbc2-9f22a5f82ffe">IVdsHwProvider::Refresh</a> 
        method to restore the cache.
       

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
The drive object no longer exists.

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
Another operation is in progress; this operation cannot proceed until the previous operation or operations 
        are complete.
       

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
The subsystem does not support this method.

</td>
</tr>
</table>
 




## -remarks



A drive can contribute extents to any number of LUNs, and these LUNs can be unmasked to any number of different
    computers on the network. Use the 
    <a href="https://msdn.microsoft.com/e9ed5bdd-c696-47cc-84c8-266b230f7970">IVdsLunPlex::QueryExtents</a> method to see all 
    the extents of a LUN plex.

The <b>LunId</b> member of each 
     <a href="https://msdn.microsoft.com/c155d925-e86f-4bec-9032-dae2221172a7">VDS_DRIVE_EXTENT</a>structure specifies the GUID for the LUN to which each allocated extent contributes. Consequently, you can use 
     the result of this method to determine the number of LUNs to which the drive contributes by counting the number 
     of distinct <b>LunId</b> values returned in <i>ppExtentArray</i>.




## -see-also




<a href="https://msdn.microsoft.com/597917cf-fb02-4949-98c3-3da3f7449ed1">IVdsDrive</a>



<a href="https://msdn.microsoft.com/aeb06a98-8896-446f-abd5-ea40be0bea40">IVdsHwProvider::Reenumerate</a>



<a href="https://msdn.microsoft.com/25ddc73c-5d1b-4bec-bbc2-9f22a5f82ffe">IVdsHwProvider::Refresh</a>



<a href="https://msdn.microsoft.com/e9ed5bdd-c696-47cc-84c8-266b230f7970">IVdsLunPlex::QueryExtents</a>



<a href="https://msdn.microsoft.com/c155d925-e86f-4bec-9032-dae2221172a7">VDS_DRIVE_EXTENT</a>
 

 

