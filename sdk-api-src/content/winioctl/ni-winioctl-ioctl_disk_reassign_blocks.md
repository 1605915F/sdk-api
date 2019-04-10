---
UID: NI:winioctl.IOCTL_DISK_REASSIGN_BLOCKS
title: IOCTL_DISK_REASSIGN_BLOCKS (winioctl.h)
author: windows-sdk-content
description: Directs the disk device to map one or more blocks to its spare-block pool.
old-location: fs\ioctl_disk_reassign_blocks.htm
tech.root: FileIO
ms.assetid: 57343bc9-9dd4-47a3-8130-07ea330eb4d3
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IOCTL_DISK_REASSIGN_BLOCKS, IOCTL_DISK_REASSIGN_BLOCKS control, IOCTL_DISK_REASSIGN_BLOCKS control code [Files], _win32_ioctl_disk_reassign_blocks, base.ioctl_disk_reassign_blocks, fs.ioctl_disk_reassign_blocks, winioctl/IOCTL_DISK_REASSIGN_BLOCKS
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
 - IOCTL_DISK_REASSIGN_BLOCKS
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCTL_DISK_REASSIGN_BLOCKS IOCTL


## -description


Directs the disk device to map one or more blocks to its spare-block pool.

To perform this operation, call the <a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a> 
    function with the following parameters.

```cpp
BOOL DeviceIoControl(
  (HANDLE) hDevice,            // handle to device
  IOCTL_DISK_REASSIGN_BLOCKS,  // dwIoControlCode(LPVOID) lpInBuffer,         // input buffer 
  (DWORD) nInBufferSize,       // size of input buffer 
  NULL,                        // lpOutBuffer0,                           // nOutBufferSize(LPDWORD) lpBytesReturned,   // number of bytes returned
  (LPOVERLAPPED) lpOverlapped  // OVERLAPPED structure
);
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



The <a href="https://msdn.microsoft.com/43d908fc-0e43-49ab-a96f-b6b0f491c99d">REASSIGN_BLOCKS</a> structure that the 
    <b>IOCTL_DISK_REASSIGN_BLOCKS</b> control code uses only 
    supports drives where the Logical Block Address (LBA) fits into a 4-byte value (typically up to 2 TB). For larger 
    drives the <a href="https://msdn.microsoft.com/48036bdc-3588-41a6-9dbb-4606bdfcb683">REASSIGN_BLOCKS_EX</a> structure that  the 
    <a href="https://msdn.microsoft.com/126ffefa-165b-4ca1-a905-1aebc8e790c7">IOCTL_DISK_REASSIGN_BLOCKS_EX</a> control code 
    uses supports 8-byte LBAs. For compatibility, the 
    <b>IOCTL_DISK_REASSIGN_BLOCKS</b> control code and 
    <b>REASSIGN_BLOCKS</b> structure should be used where 
    possible.




## -see-also




<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a>



<a href="https://msdn.microsoft.com/488a7d32-cbb5-4f32-9655-0aca8ac69640">Disk Management Control Codes</a>



<a href="https://msdn.microsoft.com/126ffefa-165b-4ca1-a905-1aebc8e790c7">IOCTL_DISK_REASSIGN_BLOCKS_EX</a>



<a href="https://msdn.microsoft.com/43d908fc-0e43-49ab-a96f-b6b0f491c99d">REASSIGN_BLOCKS</a>



<a href="https://msdn.microsoft.com/48036bdc-3588-41a6-9dbb-4606bdfcb683">REASSIGN_BLOCKS_EX</a>
 

 

