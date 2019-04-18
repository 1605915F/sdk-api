---
UID: NS:winioctl._DISK_GEOMETRY
title: DISK_GEOMETRY (winioctl.h)
author: windows-sdk-content
description: Describes the geometry of disk devices and media.
old-location: fs\disk_geometry_str.htm
tech.root: FileIO
ms.assetid: 5e5955b4-1319-42c9-9df8-9910c05dec69
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDISK_GEOMETRY, DISK_GEOMETRY, DISK_GEOMETRY structure [Files], _win32_disk_geometry_str, base.disk_geometry_str, fs.disk_geometry_str, winioctl/DISK_GEOMETRY"
ms.topic: struct
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
 - DISK_GEOMETRY
product: Windows
targetos: Windows
req.typenames: DISK_GEOMETRY, *PDISK_GEOMETRY
req.redist: 
ms.custom: 19H1
---

# DISK_GEOMETRY structure


## -description


Describes the geometry of disk devices and media.


## -struct-fields




### -field Cylinders

The number of cylinders. See <a href="https://msdn.microsoft.com/6a2985b6-5baf-49ab-af28-67c1374557ea">LARGE_INTEGER</a>.


### -field MediaType

The type of media. For a list of values, see 
<a href="https://msdn.microsoft.com/183cf8fc-c17b-4def-b590-0aa4b67488f6">MEDIA_TYPE</a>.


### -field TracksPerCylinder

The number of tracks per cylinder.


### -field SectorsPerTrack

The number of sectors per track.


### -field BytesPerSector

The number of bytes per sector.


## -see-also




<a href="https://msdn.microsoft.com/574efc29-112b-42fe-ad1b-72543f20e831">IOCTL_DISK_GET_DRIVE_GEOMETRY</a>



<a href="https://msdn.microsoft.com/67f65549-f24b-4ef2-a98f-1fc618a3bb77">IOCTL_STORAGE_GET_MEDIA_TYPES</a>



<a href="https://msdn.microsoft.com/183cf8fc-c17b-4def-b590-0aa4b67488f6">MEDIA_TYPE</a>
 

 

