---
UID: NS:winioctl._DEVICE_SEEK_PENALTY_DESCRIPTOR
title: DEVICE_SEEK_PENALTY_DESCRIPTOR
author: windows-sdk-content
description: Used in conjunction with the IOCTL_STORAGE_QUERY_PROPERTY request to retrieve the seek penalty descriptor data for a device.
old-location: fs\device_seek_penalty_descriptor.htm
tech.root: fileio
ms.assetid: b3fbf27a-dac8-4fd2-8c0d-f621f0123c98
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PDEVICE_SEEK_PENALTY_DESCRIPTOR, DEVICE_SEEK_PENALTY_DESCRIPTOR, DEVICE_SEEK_PENALTY_DESCRIPTOR structure [Files], PDEVICE_SEEK_PENALTY_DESCRIPTOR, PDEVICE_SEEK_PENALTY_DESCRIPTOR structure pointer [Files], fs.device_seek_penalty_descriptor, winioctl/DEVICE_SEEK_PENALTY_DESCRIPTOR, winioctl/PDEVICE_SEEK_PENALTY_DESCRIPTOR"
ms.topic: struct
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - DEVICE_SEEK_PENALTY_DESCRIPTOR
product: Windows
targetos: Windows
req.typenames: DEVICE_SEEK_PENALTY_DESCRIPTOR, *PDEVICE_SEEK_PENALTY_DESCRIPTOR
req.redist: 
---

# DEVICE_SEEK_PENALTY_DESCRIPTOR structure


## -description


Used in conjunction with the 
   <a href="https://msdn.microsoft.com/6755dcd4-e4a0-423f-9dcc-b9719c8e5c88">IOCTL_STORAGE_QUERY_PROPERTY</a> request to 
   retrieve the seek penalty descriptor data for a device.


## -struct-fields




### -field Version

Contains the size of this structure, in bytes. The value of this member will change as members are added to 
      the structure.


### -field Size

Specifies the total size of the data returned, in bytes. This may include data that follows this 
      structure.


### -field IncursSeekPenalty

Specifies whether the device incurs a seek penalty.


## -see-also




<a href="https://msdn.microsoft.com/dd55c570-68b5-4dc5-9fd0-a6e3277c318b">Disk Management Structures</a>



<a href="https://msdn.microsoft.com/6755dcd4-e4a0-423f-9dcc-b9719c8e5c88">IOCTL_STORAGE_QUERY_PROPERTY</a>
 

 

