---
UID: NS:winioctl.STARTING_LCN_INPUT_BUFFER
title: STARTING_LCN_INPUT_BUFFER
author: windows-sdk-content
description: Contains the starting LCN to the FSCTL_GET_VOLUME_BITMAP control code.
old-location: fs\starting_lcn_input_buffer_str.htm
tech.root: fileio
ms.assetid: 94bdb166-fe75-4851-9dbb-a1a1f5836675
ms.author: windowssdkdev
ms.date: 10/12/2018
ms.keywords: "*PSTARTING_LCN_INPUT_BUFFER, PSTARTING_LCN_INPUT_BUFFER, PSTARTING_LCN_INPUT_BUFFER structure pointer [Files], STARTING_LCN_INPUT_BUFFER, STARTING_LCN_INPUT_BUFFER structure [Files], _win32_starting_lcn_input_buffer_str, base.starting_lcn_input_buffer_str, fs.starting_lcn_input_buffer_str, winioctl/PSTARTING_LCN_INPUT_BUFFER, winioctl/STARTING_LCN_INPUT_BUFFER"
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - STARTING_LCN_INPUT_BUFFER
product: Windows
targetos: Windows
req.typenames: STARTING_LCN_INPUT_BUFFER, *PSTARTING_LCN_INPUT_BUFFER
req.redist: 
---

# STARTING_LCN_INPUT_BUFFER structure


## -description


Contains the starting LCN to the 
<a href="https://msdn.microsoft.com/80ef93ee-21a4-4766-82d2-d2ddef3ef5bb">FSCTL_GET_VOLUME_BITMAP</a> control code.


## -struct-fields




### -field StartingLcn

The LCN from which the operation should start when describing a bitmap. This member will be rounded down to a file-system-dependent rounding boundary, and that value will be returned. Its  value should be an integral multiple of eight.


## -see-also




<a href="https://msdn.microsoft.com/27ccaab7-ec89-489b-80dc-df9beb7969bc">Defragmentation</a>



<a href="https://msdn.microsoft.com/80ef93ee-21a4-4766-82d2-d2ddef3ef5bb">FSCTL_GET_VOLUME_BITMAP</a>
 

 

