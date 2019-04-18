---
UID: NI:winioctl.IOCTL_CHANGER_MOVE_MEDIUM
title: IOCTL_CHANGER_MOVE_MEDIUM (winioctl.h)
author: windows-sdk-content
description: Moves a piece of media to a destination.
old-location: base\ioctl_changer_move_medium.htm
tech.root: devio
ms.assetid: 73fa826c-ef7f-4341-838e-73e025d8d1c1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IOCTL_CHANGER_MOVE_MEDIUM, IOCTL_CHANGER_MOVE_MEDIUM control, IOCTL_CHANGER_MOVE_MEDIUM control code, _win32_ioctl_changer_move_medium, base.ioctl_changer_move_medium, winioctl/IOCTL_CHANGER_MOVE_MEDIUM
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
 - IOCTL_CHANGER_MOVE_MEDIUM
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOCTL_CHANGER_MOVE_MEDIUM IOCTL


## -description


Moves a piece of media to a destination.

To perform this operation, call the 
<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a> function with the following parameters.

```cpp
BOOL DeviceIoControl(
  (HANDLE) hDevice,             // handle to device
  IOCTL_CHANGER_MOVE_MEDIUM,    // dwIoControlCode(LPVOID) lpInBuffer,          // input buffer
  (DWORD) nInBufferSize,        // size of input buffer
  NULL,                         // lpOutBuffer0,                            // nOutBufferSize(LPDWORD) lpBytesReturned,    // number of bytes returned
  (LPOVERLAPPED) lpOverlapped   // OVERLAPPED structure
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




## -see-also




<a href="https://msdn.microsoft.com/9a837686-c081-4365-9560-be64c5d343cb">CHANGER_MOVE_MEDIUM</a>



<a href="https://msdn.microsoft.com/b3a3ffa1-e710-4d96-aff8-5b6876ab032b">Device Management Control Codes</a>



<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a>
 

 

