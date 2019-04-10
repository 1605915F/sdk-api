---
UID: NS:winioctl._RETRIEVAL_POINTER_BASE
title: RETRIEVAL_POINTER_BASE (winioctl.h)
author: windows-sdk-content
description: Contains the output for the FSCTL_GET_RETRIEVAL_POINTER_BASE control code.
old-location: fs\retrieval_pointer_base.htm
tech.root: FileIO
ms.assetid: e0a779fb-6c46-4831-95dc-968e17f86a81
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PRETRIEVAL_POINTER_BASE, PRETRIEVAL_POINTER_BASE, PRETRIEVAL_POINTER_BASE structure pointer [Files], RETRIEVAL_POINTER_BASE, RETRIEVAL_POINTER_BASE structure [Files], fs.retrieval_pointer_base, winioctl/PRETRIEVAL_POINTER_BASE, winioctl/RETRIEVAL_POINTER_BASE"
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
 - RETRIEVAL_POINTER_BASE
product: Windows
targetos: Windows
req.typenames: RETRIEVAL_POINTER_BASE, *PRETRIEVAL_POINTER_BASE
req.redist: 
---

# RETRIEVAL_POINTER_BASE structure


## -description


Contains the output for the <a href="https://msdn.microsoft.com/17925fe8-ab5a-4bfb-8d9e-cd574c024107">FSCTL_GET_RETRIEVAL_POINTER_BASE</a> control code.


## -struct-fields




### -field FileAreaOffset

The volume-relative sector offset to the first allocatable unit on the file system, also referred to as the base of the cluster heap.


## -see-also




<a href="https://msdn.microsoft.com/17925fe8-ab5a-4bfb-8d9e-cd574c024107">FSCTL_GET_RETRIEVAL_POINTER_BASE</a>
 

 

