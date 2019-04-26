---
UID: NS:winioctl._SET_PARTITION_INFORMATION
title: SET_PARTITION_INFORMATION
author: windows-sdk-content
description: Contains information used to set a disk partition's type.
old-location: fs\set_partition_information_str.htm
tech.root: FileIO
ms.assetid: cc04868c-cb9c-455f-a0df-bde6a133eb60
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PSET_PARTITION_INFORMATION, PSET_PARTITION_INFORMATION, PSET_PARTITION_INFORMATION structure pointer [Files], SET_PARTITION_INFORMATION, SET_PARTITION_INFORMATION structure [Files], SET_PARTITION_INFORMATION_MBR, _win32_set_partition_information_str, base.set_partition_information_str, fs.set_partition_information_str, winioctl/PSET_PARTITION_INFORMATION, winioctl/SET_PARTITION_INFORMATION"
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
 - SET_PARTITION_INFORMATION
product: Windows
targetos: Windows
req.typenames: SET_PARTITION_INFORMATION, *PSET_PARTITION_INFORMATION
req.redist: 
---

# SET_PARTITION_INFORMATION structure


## -description


Contains information used to set a disk partition's type.
<div class="alert"><b>Note</b>  <b>SET_PARTITION_INFORMATION</b> has been superseded by the 
<a href="https://msdn.microsoft.com/3c88ebae-274e-403a-8f57-58fdf863f511">PARTITION_INFORMATION_EX</a> structure.</div><div> </div>

## -struct-fields




### -field PartitionType

The type of partition. For a list of values, see 
<a href="https://msdn.microsoft.com/b2e15b93-a02b-4d6f-b242-b5ec9a30c97b">Disk Partition Types</a>.


## -see-also




<a href="https://msdn.microsoft.com/24053a1a-8cf8-4aa8-a611-15c9fae0a36d">IOCTL_DISK_GET_PARTITION_INFO</a>



<a href="https://msdn.microsoft.com/868cad92-fa88-4a5a-98bb-92e73c115a22">IOCTL_DISK_SET_PARTITION_INFO</a>



<a href="https://msdn.microsoft.com/3c88ebae-274e-403a-8f57-58fdf863f511">PARTITION_INFORMATION_EX</a>
 

 

