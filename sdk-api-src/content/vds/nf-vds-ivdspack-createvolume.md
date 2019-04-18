---
UID: NF:vds.IVdsPack.CreateVolume
title: IVdsPack::CreateVolume (vds.h)
author: windows-sdk-content
description: Creates a volume within the pack.
old-location: base\ivdspack_createvolume.htm
tech.root: VDS
ms.assetid: 26fea1a4-f060-49e2-a7ac-0e751f798c72
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CreateVolume, CreateVolume method [VDS], CreateVolume method [VDS],IVdsPack interface, IVdsPack interface [VDS],CreateVolume method, IVdsPack.CreateVolume, IVdsPack::CreateVolume, base.ivdspack_createvolume, vds/IVdsPack::CreateVolume
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
 - IVdsPack.CreateVolume
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVdsPack::CreateVolume


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Creates a volume within the pack. The interface pointer for the new 
   <a href="https://msdn.microsoft.com/92013015-b0f5-4b92-937b-c2637f65810c">volume object</a> can be retrieved by calling 
   <a href="https://msdn.microsoft.com/1bb30247-efb8-488f-b142-8912c351f5f2">IVdsAsync::Wait</a> through the 
   <i>ppAsync</i> parameter. The 
   <a href="https://msdn.microsoft.com/21771c6a-eca9-47f3-b6fc-383bca1e11bf">VDS_ASYNC_OUTPUT</a> structure returned contains the volume 
   object interface pointer in the <b>cv.pVolumeUnk</b> member.


## -parameters




### -param type [in]

A volume type enumerated by <a href="https://msdn.microsoft.com/07a44bbf-0726-4094-9b5f-2d26b0030796">VDS_VOLUME_TYPE</a>. 
      Volumes on basic disks can have only one extent, and only the <b>VDS_VT_SIMPLE</b> flag is 
      valid.


### -param pInputDiskArray [in]

Pointer to an array of <a href="https://msdn.microsoft.com/837981e5-8600-4add-85cf-a802615133d3">VDS_INPUT_DISK</a> 
      structures; one structure for each disk. A disk can be included in the array only once. All disks in the array 
      must be used, or the method fails. Callers must allocate and initialize the array, and free the memory when the 
      call returns.


### -param lNumberOfDisks [in]

The total number of disks contributing to the volume. 
      

<div class="alert"><b>Note</b>  VDS imposes a 32-disk limit on spanned, striped, and striped with parity (RAID-5) volumes.</div>
<div> </div>

### -param ulStripeSize [in]

If the volume is striped, the size of each stripe in bytes. Pass in zero bytes for 
      <b>VDS_VT_SIMPLE</b>, <b>VDS_VT_SPAN</b>, and 
      <b>VDS_VT_MIRROR</b>; 64 kilobytes for <b>VDS_VT_STRIPE</b> and 
      <b>VDS_VT_PARITY</b>.


### -param ppAsync [out]

The address of an <a href="https://msdn.microsoft.com/7814b8ef-84b4-453e-b480-c32b67e5af93">IVdsAsync</a> interface pointer, 
      which VDS initializes on return. Callers must release the interface. Use this pointer to cancel, wait for, 
      or query the status of the operation.

If you call <a href="https://msdn.microsoft.com/1bb30247-efb8-488f-b142-8912c351f5f2">IVdsAsync::Wait</a> on this method and a success HRESULT value is returned, 
      you must release the interfaces returned in the 
      <a href="https://msdn.microsoft.com/21771c6a-eca9-47f3-b6fc-383bca1e11bf">VDS_ASYNC_OUTPUT</a> structure by calling the <a href="https://msdn.microsoft.com/en-us/library/ms682317(v=VS.85).aspx">IUnknown::Release</a> method on each interface pointer. However, if <b>Wait</b> returns a failure HRESULT value, or if the <i>pHrResult</i> parameter of <b>Wait</b> receives a failure HRESULT value, the interface pointers in the <b>VDS_ASYNC_OUTPUT</b> structure are <b>NULL</b> and do not need to be released. You can test for success or failure HRESULT values by using the <a href="https://msdn.microsoft.com/en-us/library/ms687197(v=VS.85).aspx">SUCCEEDED</a> and <a href="https://msdn.microsoft.com/en-us/library/ms693474(v=VS.85).aspx">FAILED</a> macros defined in Winerror.h.


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
The volume was created successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_S_NO_NOTIFICATION</b></dt>
<dt>0x00042517L</dt>
</dl>
</td>
<td width="60%">
No volume arrival notification was received. You may need to call <a href="https://msdn.microsoft.com/ca6a1143-b5f0-49e5-8505-836c565aabcf">IVdsService::Refresh</a>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_S_UPDATE_BOOTFILE_FAILED</b></dt>
<dt>0x00042434L</dt>
</dl>
</td>
<td width="60%">
The volume is created successfully, but VDS failed to update the boot options in the Boot Configuration Data (BCD) store.

<b>Windows Server 2003:  </b>Boot options are stored in the boot.ini file on an x86 or x64 system 
        or NVRAM on an Itanium system.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_DISK_NOT_FOUND_IN_PACK</b></dt>
<dt>0x8004252DL</dt>
</dl>
</td>
<td width="60%">
The specified disks do not belong to the same pack.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_DMADMIN_METHOD_CALL_FAILED</b></dt>
<dt>0x80042420L</dt>
</dl>
</td>
<td width="60%">
LDM service failed a method.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_EXTENT_SIZE_LESS_THAN_MIN</b></dt>
<dt>0x80042433L</dt>
</dl>
</td>
<td width="60%">
Extent size passed in is too small.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_DISK_COUNT</b></dt>
<dt>0x80042526L</dt>
</dl>
</td>
<td width="60%">
The number of disks specified is not valid for this operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_MEMBER_COUNT</b></dt>
<dt>0x80042522L</dt>
</dl>
</td>
<td width="60%">
The member count for the volume must be greater than zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_MEMBER_ORDER</b></dt>
<dt>0x80042524L</dt>
</dl>
</td>
<td width="60%">
The member indexes must be monotonically increasing and begin with zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_OPERATION</b></dt>
<dt>0x80042415L</dt>
</dl>
</td>
<td width="60%">
The disk passed in is a CD-ROM or DVD device.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_PACK</b></dt>
<dt>0x8004251AL</dt>
</dl>
</td>
<td width="60%">
This operation is not allowed on this disk pack.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_PLEX_COUNT</b></dt>
<dt>0x80042521L</dt>
</dl>
</td>
<td width="60%">
The plex count for the volume must be greater than zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_PLEX_ORDER</b></dt>
<dt>0x80042523L</dt>
</dl>
</td>
<td width="60%">
The plex indexes must be monotonically increasing and begin with zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_INVALID_STRIPE_SIZE</b></dt>
<dt>0x80042525L</dt>
</dl>
</td>
<td width="60%">
The stripe size in bytes must be a power of 2 for striped and RAID-5 volume types and must be zero for all other volume types.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_MISSING_DISK</b></dt>
<dt>0x80042454L</dt>
</dl>
</td>
<td width="60%">
The specified disk is missing.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_NO_MEDIA</b></dt>
<dt>0x80042412L</dt>
</dl>
</td>
<td width="60%">
There is no media in a removable drive passed in through the disk array.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_NOT_ENOUGH_SPACE</b></dt>
<dt>0x8004240FL</dt>
</dl>
</td>
<td width="60%">
There is not enough space on one of the disks.

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
The volume type is not supported, or a volume already exists on the removable disk passed into the method. A removable disk can have only one 
        volume.

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
At least one of the disks passed in is not found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_ONE_EXTENT_PER_DISK</b></dt>
<dt>0x80042531L</dt>
</dl>
</td>
<td width="60%">
A single disk cannot contribute to multiple members or multiple plexes of the same volume.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_PACK_OFFLINE</b></dt>
<dt>0x80042444L</dt>
</dl>
</td>
<td width="60%">
The target pack is inaccessible.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_PARTITION_LIMIT_REACHED</b></dt>
<dt>0x80042407L</dt>
</dl>
</td>
<td width="60%">
The maximum number of partitions (primary partitions or primary partitions with an extended partition) 
        already exists when the caller tries to create an additional primary partition or extended partition.

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
The dynamic provider cache is corrupt.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_VOLUME_DISK_COUNT_MAX_EXCEEDED</b></dt>
<dt>0x80042529L</dt>
</dl>
</td>
<td width="60%">
No more than 32 disks are allowed per volume.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VDS_E_VOLUME_TOO_SMALL</b></dt>
<dt>0x8004242CL</dt>
</dl>
</td>
<td width="60%">
The volume size is too small.

</td>
</tr>
</table>
 




## -remarks



<div class="alert"><b>Note</b>  This method cannot be used to create a volume on a removable disk.</div>
<div> </div>
Callers use this method to create a new simple, spanned, striped, mirrored, or striped with 
    parity (RAID-5) volume in the current pack. Simple and spanned volumes have exactly one plex and one member. 
    Striped and RAID-5 volumes have multiple columns and members. Mirrored volumes consist of multiple plexes.

Basic disks can contain only simple volumes. Dynamic disks can contain volumes of all types as 
    long as the operating system supports the binding operation; non-server platforms do not support fault-tolerant 
    binding operations. All newly created volumes lack a drive letter.

On a basic disk, this method creates a primary partition. If there are already three primary partitions on the disk, it creates an extended partition to cover the largest contiguous free disk space extent left on the disk, and then creates a logical drive within the extended partition.

A disk cannot contribute to more than one plex of the same volume; however, a single disk can 
    contribute to multiple volumes. A simple volume has only one 
    <a href="https://msdn.microsoft.com/837981e5-8600-4add-85cf-a802615133d3">VDS_INPUT_DISK</a> structure, whereas, spanned, striped, 
    mirrored, and RAID-5 volumes have one structure for each contributing disk.

The size of the disk specified in the 
    <a href="https://msdn.microsoft.com/837981e5-8600-4add-85cf-a802615133d3">VDS_INPUT_DISK</a> structure  can be the full disk or a 
    portion of the disk. When two disks form a mirrored volume, VDS uses the smallest disk to calculate the size of 
    the mirror. (Provider policy determines the actual offset, length, and number of disk extents allocated on a 
    given input disk.) Use the 
    <a href="https://msdn.microsoft.com/43f9972d-14a6-4674-bf90-741ad3a9eb0d">IVdsPack::QueryVolumes</a> method to  determine 
    the exact size of the created volume.

To create a logical volume with an optional alignment parameter, use the <a href="https://msdn.microsoft.com/cc7de88b-af6c-4d39-9297-49e33810466a">IVdsPack2::CreateVolume2</a> method or use the <b>HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\vds\Alignment</b> registry key to specify the alignment value in bytes.

<b>Windows 7, Windows Server 2008 R2, Windows Vista and Windows Server 2008:  </b>On a basic disk, the CreateVolume method ignores the <b>HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\vds\Alignment</b> registry key. This is a known issue and is being addressed. As a workaround, use the <a href="https://msdn.microsoft.com/94f80a9f-459f-4f3d-8d85-e5ec7d5734c4">IVdsAdvancedDisk::CreatePartition</a>  or <a href="https://msdn.microsoft.com/c9ab5a24-b0b3-41cc-a4bf-3619f156008c">IVdsCreatePartitionEx::CreatePartitionEx</a> method to create partitions on the basic disk so that they are aligned correctly.<p class="note">Dynamic partitions and volumes are aligned using the values under the following registry key:

<p class="note"><b>HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\vds\Alignment</b>

<p class="note">The default alignment is 1 MB if the disk is 4 GB or larger, or 64 KB if the disk is smaller than 4 GB.



Implementers must return a pointer to the <a href="https://msdn.microsoft.com/7814b8ef-84b4-453e-b480-c32b67e5af93">IVdsAsync</a> 
    interface for this method, regardless of whether the call initiates an asynchronous operation.




## -see-also




<a href="https://msdn.microsoft.com/7814b8ef-84b4-453e-b480-c32b67e5af93">IVdsAsync</a>



<a href="https://msdn.microsoft.com/1bb30247-efb8-488f-b142-8912c351f5f2">IVdsAsync::Wait</a>



<a href="https://msdn.microsoft.com/106989fe-d1dd-4c7f-b889-00a671c6e567">IVdsPack</a>



<a href="https://msdn.microsoft.com/cc7de88b-af6c-4d39-9297-49e33810466a">IVdsPack2::CreateVolume2</a>



<a href="https://msdn.microsoft.com/43f9972d-14a6-4674-bf90-741ad3a9eb0d">IVdsPack::QueryVolumes</a>



<a href="https://msdn.microsoft.com/21771c6a-eca9-47f3-b6fc-383bca1e11bf">VDS_ASYNC_OUTPUT</a>



<a href="https://msdn.microsoft.com/837981e5-8600-4add-85cf-a802615133d3">VDS_INPUT_DISK</a>



<a href="https://msdn.microsoft.com/07a44bbf-0726-4094-9b5f-2d26b0030796">VDS_VOLUME_TYPE</a>
 

 

