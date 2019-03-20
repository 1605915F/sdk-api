---
UID: NI:winioctl.IOCTL_STORAGE_SET_HOTPLUG_INFO
title: IOCTL_STORAGE_SET_HOTPLUG_INFO (winioctl.h)
author: windows-sdk-content
description: Sets the hotplug configuration of the specified device.
old-location: base\ioctl_storage_set_hotplug_info.htm
tech.root: devio
ms.assetid: f15c183d-d883-470c-9b78-e63d2a9b76ca
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOCTL_STORAGE_SET_HOTPLUG_INFO, IOCTL_STORAGE_SET_HOTPLUG_INFO control, IOCTL_STORAGE_SET_HOTPLUG_INFO control code, _win32_ioctl_storage_set_hotplug_info, base.ioctl_storage_set_hotplug_info, winioctl/IOCTL_STORAGE_SET_HOTPLUG_INFO
ms.topic: ioctl
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
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
 - IOCTL_STORAGE_SET_HOTPLUG_INFO
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCTL_STORAGE_SET_HOTPLUG_INFO IOCTL


## -description


Sets the hotplug configuration of the specified device.

To perform this operation, call the 
<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a> function with the following parameters.

```cpp
BOOL DeviceIoControl(
  (HANDLE) hDevice,                // handle to device
  IOCTL_STORAGE_SET_HOTPLUG_INFO,  // dwIoControlCode(LPVOID) lpInBuffer,             // input buffer
  (DWORD) nInBufferSize,           // size of input buffer
  NULL,                            // lpOutBuffer0,                               // nOutBufferSize(LPDWORD) lpBytesReturned,       // number of bytes returned
  (LPOVERLAPPED) lpOverlapped      // OVERLAPPED structure
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



Refer to the Remarks section in the reference page for 
<a href="https://msdn.microsoft.com/861e6067-9f37-427a-8d3b-8cb9d0f95c40">STORAGE_HOTPLUG_INFO</a> for more information about hotplug devices.

This operation sets only the <b>DeviceHotplug</b> member of the 
<a href="https://msdn.microsoft.com/861e6067-9f37-427a-8d3b-8cb9d0f95c40">STORAGE_HOTPLUG_INFO</a> structure passed in.




## -see-also




<a href="https://msdn.microsoft.com/b3a3ffa1-e710-4d96-aff8-5b6876ab032b">Device Management Control Codes</a>



<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a>



<a href="https://msdn.microsoft.com/4ecf6f84-17fc-4c48-a859-c043e8f9cd14">IOCTL_STORAGE_GET_HOTPLUG_INFO</a>



<a href="https://msdn.microsoft.com/861e6067-9f37-427a-8d3b-8cb9d0f95c40">STORAGE_HOTPLUG_INFO</a>
 

 

