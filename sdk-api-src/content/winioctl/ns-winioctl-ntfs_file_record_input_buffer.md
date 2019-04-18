---
UID: NS:winioctl.__unnamed_struct_8
title: NTFS_FILE_RECORD_INPUT_BUFFER (winioctl.h)
author: windows-sdk-content
description: Contains data for the FSCTL_GET_NTFS_FILE_RECORD control code.
old-location: fs\ntfs_file_record_input_buffer_str.htm
tech.root: FileIO
ms.assetid: 8b0317ca-6d0e-4a04-a05a-1627d22171e3
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PNTFS_FILE_RECORD_INPUT_BUFFER, NTFS_FILE_RECORD_INPUT_BUFFER, NTFS_FILE_RECORD_INPUT_BUFFER structure [Files], PNTFS_FILE_RECORD_INPUT_BUFFER, PNTFS_FILE_RECORD_INPUT_BUFFER structure pointer [Files], _win32_ntfs_file_record_input_buffer_str, base.ntfs_file_record_input_buffer_str, fs.ntfs_file_record_input_buffer_str, winioctl/NTFS_FILE_RECORD_INPUT_BUFFER, winioctl/PNTFS_FILE_RECORD_INPUT_BUFFER"
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
 - NTFS_FILE_RECORD_INPUT_BUFFER
product: Windows
targetos: Windows
req.typenames: NTFS_FILE_RECORD_INPUT_BUFFER, *PNTFS_FILE_RECORD_INPUT_BUFFER
req.redist: 
ms.custom: 19H1
---

# NTFS_FILE_RECORD_INPUT_BUFFER structure


## -description


Contains data for the 
<a href="https://msdn.microsoft.com/a7308fa4-0f69-4b69-bb89-5d645e2a9f6e">FSCTL_GET_NTFS_FILE_RECORD</a> control code.


## -struct-fields




### -field FileReferenceNumber

The file identifier of the file record to be retrieved. This is not necessarily the file identifier returned in the <b>FileReferenceNumber</b> member of the 
<a href="https://msdn.microsoft.com/e2597939-5159-4c35-9a1f-f3be43081d72">NTFS_FILE_RECORD_OUTPUT_BUFFER</a> structure. Refer to the Remarks section of the reference page for 
<a href="https://msdn.microsoft.com/a7308fa4-0f69-4b69-bb89-5d645e2a9f6e">FSCTL_GET_NTFS_FILE_RECORD</a> for more information.
					


## -remarks



Pass this structure as input to the 
<a href="https://msdn.microsoft.com/a7308fa4-0f69-4b69-bb89-5d645e2a9f6e">FSCTL_GET_NTFS_FILE_RECORD</a> control code.




## -see-also




<a href="https://msdn.microsoft.com/a7308fa4-0f69-4b69-bb89-5d645e2a9f6e">FSCTL_GET_NTFS_FILE_RECORD</a>



<a href="https://msdn.microsoft.com/e2597939-5159-4c35-9a1f-f3be43081d72">NTFS_FILE_RECORD_OUTPUT_BUFFER</a>
 

 

