---
UID: NI:winioctl.IOCTL_DISK_GET_PARTITION_INFO
title: IOCTL_DISK_GET_PARTITION_INFO (winioctl.h)
author: windows-sdk-content
description: Retrieves information about the type, size, and nature of a disk partition.
old-location: fs\ioctl_disk_get_partition_info.htm
tech.root: FileIO
ms.assetid: 24053a1a-8cf8-4aa8-a611-15c9fae0a36d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IOCTL_DISK_GET_PARTITION_INFO, IOCTL_DISK_GET_PARTITION_INFO control, IOCTL_DISK_GET_PARTITION_INFO control code [Files], _win32_ioctl_disk_get_partition_info, base.ioctl_disk_get_partition_info, fs.ioctl_disk_get_partition_info, winioctl/IOCTL_DISK_GET_PARTITION_INFO
ms.topic: ioctl
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
 - HeaderDef
api_location:
 - WinIoCtl.h
api_name:
 - IOCTL_DISK_GET_PARTITION_INFO
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOCTL_DISK_GET_PARTITION_INFO IOCTL


## -description


Retrieves information about the type, size, and nature of a disk partition.
<div class="alert"><b>Note</b>  <b>IOCTL_DISK_GET_PARTITION_INFO</b> is superseded by 
    <a href="https://msdn.microsoft.com/f84f8be6-2b01-4a20-8669-cb1a55c32907">IOCTL_DISK_GET_PARTITION_INFO_EX</a>, which 
    retrieves partition information for AT and Extensible Firmware Interface (EFI) partitions.</div><div> </div>To perform this operation, call the 
    <a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a> function with the following 
    parameters.

```cpp
BOOL DeviceIoControl( (HANDLE) hDevice,                // handle to a partition
                      IOCTL_DISK_GET_PARTITION_INFO,   // dwIoControlCode(LPVOID) NULL,                   // lpInBuffer(DWORD) 0,                       // nInBufferSize(LPVOID) lpOutBuffer,            // output buffer
                      (DWORD) nOutBufferSize,          // size of output buffer
                      (LPDWORD) lpBytesReturned,       // number of bytes returned
                      (LPOVERLAPPED) lpOverlapped );   // OVERLAPPED structure
```



## -ioctlparameters




### -input-buffer



<text></text>




### -input-buffer-length



<text></text>




### -output-buffer



<text></text>




### -output-buffer-length



<text></text>




### -in-out-buffer



<text></text>




### -inout-buffer-length



<text></text>




### -status-block



Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.

Otherwise, Status to the appropriate error condition as a NTSTATUS code. 

For more information, see [NTSTATUS Values](https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/ntstatus-values).




## -remarks



The <b>IOCTL_DISK_GET_PARTITION_INFO</b> 
    control code is only supported on MBR-formatted disks.

The disk support can be summarized as follows.

<table>
<tr>
<th>Disk type</th>
<th>IOCTL_DISK_GET_PARTITION_INFO</th>
<th>IOCTL_DISK_GET_PARTITION_INFO_EX</th>
</tr>
<tr>
<td>Basic master boot record (MBR)</td>
<td>Yes</td>
<td>Yes</td>
</tr>
<tr>
<td>Basic GUID partition table (GPT)</td>
<td>No</td>
<td>Yes</td>
</tr>
<tr>
<td>Dynamic MBR boot/system</td>
<td>Yes</td>
<td>Yes</td>
</tr>
<tr>
<td>Dynamic MBR data</td>
<td>Yes</td>
<td>No</td>
</tr>
<tr>
<td>Dynamic GPT boot/system</td>
<td>No</td>
<td>Yes</td>
</tr>
<tr>
<td>Dynamic GPT data</td>
<td>No</td>
<td>No</td>
</tr>
</table>
 

Currently, GPT is supported only on 64-bit systems.

If the partition is on a disk formatted as type master boot record (MBR), partition size totals are limited. 
    For more information, see the Remarks section of 
    <a href="https://msdn.microsoft.com/8cace6a5-666a-4d35-a557-6bf0564dbe58">IOCTL_DISK_SET_DRIVE_LAYOUT</a>.




## -see-also




<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a>



<a href="https://msdn.microsoft.com/488a7d32-cbb5-4f32-9655-0aca8ac69640">Disk Management Control Codes</a>



<a href="https://msdn.microsoft.com/a5b1e97c-f22a-4d90-a3f4-1589ad9d1cc3">File System Recognition</a>



<a href="https://msdn.microsoft.com/f84f8be6-2b01-4a20-8669-cb1a55c32907">IOCTL_DISK_GET_PARTITION_INFO_EX</a>



<a href="https://msdn.microsoft.com/868cad92-fa88-4a5a-98bb-92e73c115a22">IOCTL_DISK_SET_PARTITION_INFO</a>



<a href="https://msdn.microsoft.com/2c8fa83a-0694-4e17-a9e4-87f839a0d458">PARTITION_INFORMATION</a>
 

 

