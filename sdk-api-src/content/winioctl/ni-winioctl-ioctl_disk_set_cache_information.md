---
UID: NI:winioctl.IOCTL_DISK_SET_CACHE_INFORMATION
title: IOCTL_DISK_SET_CACHE_INFORMATION
author: windows-sdk-content
description: Sets the disk configuration data.
old-location: fs\ioctl_disk_set_cache_information.htm
tech.root: fileio
ms.assetid: e921da48-9435-41f0-87dd-abb383fd5208
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOCTL_DISK_SET_CACHE_INFORMATION, IOCTL_DISK_SET_CACHE_INFORMATION control, IOCTL_DISK_SET_CACHE_INFORMATION control code [Files], base.ioctl_disk_set_cache_information, fs.ioctl_disk_set_cache_information, winioctl/IOCTL_DISK_SET_CACHE_INFORMATION
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
 - IOCTL_DISK_SET_CACHE_INFORMATION
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCTL_DISK_SET_CACHE_INFORMATION IOCTL


## -description


Sets the disk configuration data.

To perform this operation, call the 
<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a> function with the following parameters.

```cpp
BOOL DeviceIoControl(
  (HANDLE) hDevice,                 // handle to device
  IOCTL_DISK_SET_CACHE_INFORMATION, // dwIoControlCode(LPVOID) lpInBuffer,              // input buffer
  (DWORD) nInBufferSize,            // size of input buffer
  NULL,                             // lpOutBuffer0,                                // nOutBufferSize(LPDWORD) lpBytesReturned,        // number of bytes returned
  (LPOVERLAPPED) lpOverlapped       // OVERLAPPED structure
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



To retrieve the cache information, use the 
    <a href="https://msdn.microsoft.com/025a92e8-6169-4d7e-9029-f22acb2bdc9f">IOCTL_DISK_GET_CACHE_INFORMATION</a> control code.




## -see-also




<a href="https://msdn.microsoft.com/ea175bea-5f2b-4f3e-9fe0-239b1d2e3d96">DISK_CACHE_INFORMATION</a>



<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a>



<a href="https://msdn.microsoft.com/488a7d32-cbb5-4f32-9655-0aca8ac69640">Disk
		  Management Control Codes</a>



<a href="https://msdn.microsoft.com/025a92e8-6169-4d7e-9029-f22acb2bdc9f">IOCTL_DISK_GET_CACHE_INFORMATION</a>
 

 

