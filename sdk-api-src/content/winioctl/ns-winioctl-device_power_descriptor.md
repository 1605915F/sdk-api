---
UID: NS:winioctl._DEVICE_POWER_DESCRIPTOR
title: DEVICE_POWER_DESCRIPTOR (winioctl.h)
author: windows-sdk-content
description: The DEVICE_POWER_DESCRIPTOR structure describes the power capabilities of a storage device.
old-location: fs\device_power_descriptor.htm
tech.root: FileIO
ms.assetid: 63e51485-db3f-45ed-925e-0abf105c8aef
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDEVICE_POWER_DESCRIPTOR, DEVICE_POWER_DESCRIPTOR, DEVICE_POWER_DESCRIPTOR structure [Storage Devices], PDEVICE_POWER_DESCRIPTOR, PDEVICE_POWER_DESCRIPTOR structure pointer [Storage Devices], fs.device_power_descriptor, fs.device_zero_power_odd_descriptor, winioctl/DEVICE_POWER_DESCRIPTOR, winioctl/PDEVICE_POWER_DESCRIPTOR"
ms.topic: struct
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - DEVICE_POWER_DESCRIPTOR
product: Windows
targetos: Windows
req.typenames: DEVICE_POWER_DESCRIPTOR, *PDEVICE_POWER_DESCRIPTOR
req.redist: 
ms.custom: 19H1
---

# DEVICE_POWER_DESCRIPTOR structure


## -description


The <b>DEVICE_POWER_DESCRIPTOR</b> 
    structure describes the power capabilities of a storage device.


## -struct-fields




### -field Version

Contains the size of this structure, in bytes. The value of this member will change as members are added to 
      the structure.


### -field Size

Specifies the total size of the data returned, in bytes. This may include data that follows this 
      structure.


### -field DeviceAttentionSupported

True if device attention is supported. Otherwise, false.


### -field AsynchronousNotificationSupported

True if the device supports asynchronous notifications, delivered via 
      <b>IOCTL_STORAGE_EVENT_NOTIFICATION</b>. Otherwise, false.


### -field IdlePowerManagementEnabled

True if the device has been registered for runtime idle power management. Otherwise, false.


### -field D3ColdEnabled

True if the device will be powered off when put into D3 power state. Otherwise, false.


### -field D3ColdSupported

True if the platform supports <b>D3ColdEnabled</b> for this device. Otherwise, 
      false.


### -field NoVerifyDuringIdlePower

 


### -field Reserved

Reserved.


### -field IdleTimeoutInMS

The idle timeout value in milliseconds. This member is ignored unless 
      <b>IdlePowerManagementEnabled</b> is true.


## -see-also




<a href="https://msdn.microsoft.com/dd55c570-68b5-4dc5-9fd0-a6e3277c318b">Disk Management Structures</a>



<a href="https://msdn.microsoft.com/6755dcd4-e4a0-423f-9dcc-b9719c8e5c88">IOCTL_STORAGE_QUERY_PROPERTY</a>



<a href="https://msdn.microsoft.com/c97a14ab-628c-41f1-96c3-0f47654d0606">STORAGE_PROPERTY_QUERY</a>
 

 

