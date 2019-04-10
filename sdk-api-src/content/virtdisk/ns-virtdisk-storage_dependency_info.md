---
UID: NS:virtdisk._STORAGE_DEPENDENCY_INFO
title: STORAGE_DEPENDENCY_INFO (virtdisk.h)
author: windows-sdk-content
description: Contains virtual hard disk (VHD) storage dependency information.
old-location: vhd\storage_dependency_info.htm
tech.root: VStor
ms.assetid: 67648a4d-3f66-407e-9036-c7072bc7e460
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PSTORAGE_DEPENDENCY_INFO, PSTORAGE_DEPENDENCY_INFO, PSTORAGE_DEPENDENCY_INFO structure pointer [VHD], STORAGE_DEPENDENCY_INFO, STORAGE_DEPENDENCY_INFO structure [VHD], _STORAGE_DEPENDENCY_INFO, vdssys/PSTORAGE_DEPENDENCY_INFO, vdssys/STORAGE_DEPENDENCY_INFO, vhd.storage_dependency_info, virtdisk/PSTORAGE_DEPENDENCY_INFO, virtdisk/STORAGE_DEPENDENCY_INFO"
ms.topic: struct
req.header: virtdisk.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
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
 - VirtDisk.h
 - vdssys.h
api_name:
 - STORAGE_DEPENDENCY_INFO
product: Windows
targetos: Windows
req.typenames: STORAGE_DEPENDENCY_INFO, *PSTORAGE_DEPENDENCY_INFO
req.redist: 
---

# STORAGE_DEPENDENCY_INFO structure


## -description


Contains virtual hard disk (VHD) storage dependency information.


## -struct-fields




### -field Version

A <a href="https://msdn.microsoft.com/en-us/library/Dd323691(v=VS.85).aspx">STORAGE_DEPENDENCY_INFO_VERSION</a> enumeration that specifies the version of the information structure being passed to or from  the VHD functions. Can be <a href="https://msdn.microsoft.com/en-us/library/Dd323689(v=VS.85).aspx">STORAGE_DEPENDENCY_INFO_TYPE_1</a> or <a href="https://msdn.microsoft.com/en-us/library/Dd323690(v=VS.85).aspx">STORAGE_DEPENDENCY_INFO_TYPE_2</a>.


### -field NumberEntries

Number of entries returned in the following unioned members.


### -field Version1Entries

Variable-length array containing <a href="https://msdn.microsoft.com/en-us/library/Dd323689(v=VS.85).aspx">STORAGE_DEPENDENCY_INFO_TYPE_1</a> structures.


### -field Version2Entries

Variable-length array containing <a href="https://msdn.microsoft.com/en-us/library/Dd323690(v=VS.85).aspx">STORAGE_DEPENDENCY_INFO_TYPE_2</a> structures.


## -see-also




<a href="https://msdn.microsoft.com/c9531c07-ad55-42b6-8685-7f55a47e8485">About VHD</a>



<a href="https://msdn.microsoft.com/3b5d0da0-2b23-4b7c-b007-ed3fe030926c">VHD Reference</a>
 

 

