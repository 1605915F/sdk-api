---
UID: NF:vds.IVdsAdvancedDisk.GetPartitionProperties
title: IVdsAdvancedDisk::GetPartitionProperties
author: windows-sdk-content
description: Returns the properties of the partition identified by the partition offset.
old-location: base\ivdsadvanceddisk_getpartitionproperties.htm
tech.root: VDS
ms.assetid: 6dc96e7b-34e5-4366-8804-d40f111d77c2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPartitionProperties, GetPartitionProperties method [VDS], GetPartitionProperties method [VDS],IVdsAdvancedDisk interface, IVdsAdvancedDisk interface [VDS],GetPartitionProperties method, IVdsAdvancedDisk.GetPartitionProperties, IVdsAdvancedDisk::GetPartitionProperties, base.ivdsadvanceddisk_getpartitionproperties, vds/IVdsAdvancedDisk::GetPartitionProperties
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Vds.h
api_name:
 - IVdsAdvancedDisk.GetPartitionProperties
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsAdvancedDisk::GetPartitionProperties


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Returns the properties of the partition identified by the partition offset.


## -parameters




### -param ullOffset [in]

The partition offset.


### -param pPartitionProp [out]

The address of the <a href="https://msdn.microsoft.com/f1b465ad-f03b-4ce8-ae83-f8e93b7fa4c4">VDS_PARTITION_PROP</a>structure allocated and passed in by the caller.


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
<dt><b>VDS_E_OBJECT_NOT_FOUND</b></dt>
<dt>0x80042405L</dt>
</dl>
</td>
<td width="60%">
The partition does not exist.

</td>
</tr>
</table>
 




## -remarks



This method returns information for all partition types.




## -see-also




<a href="https://msdn.microsoft.com/65e14273-8127-4667-b5c8-362ad54b4782">Disk Object</a>



<a href="https://msdn.microsoft.com/6b5e1bff-e7e8-4403-99ff-6dc97d113f37">IVdsAdvancedDisk</a>



<a href="https://msdn.microsoft.com/f1b465ad-f03b-4ce8-ae83-f8e93b7fa4c4">VDS_PARTITION_PROP</a>
 

 

