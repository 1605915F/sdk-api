---
UID: NS:winioctl._CHANGER_ELEMENT_LIST
title: CHANGER_ELEMENT_LIST (winioctl.h)
author: windows-sdk-content
description: Represents a range of elements of a single type, typically for an operation such as getting or initializing the status of multiple elements.
old-location: base\changer_element_list_str.htm
tech.root: devio
ms.assetid: cb1fcf78-b36a-4551-8eeb-da58edc80890
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PCHANGER_ELEMENT_LIST, CHANGER_ELEMENT_LIST, CHANGER_ELEMENT_LIST structure, PCHANGER_ELEMENT_LIST, PCHANGER_ELEMENT_LIST structure pointer, _win32_changer_element_list_str, base.changer_element_list_str, winioctl/CHANGER_ELEMENT_LIST, winioctl/PCHANGER_ELEMENT_LIST"
ms.topic: struct
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
 - CHANGER_ELEMENT_LIST
product: Windows
targetos: Windows
req.typenames: CHANGER_ELEMENT_LIST, *PCHANGER_ELEMENT_LIST
req.redist: 
---

# CHANGER_ELEMENT_LIST structure


## -description


Represents a range of elements of a single type, typically for an operation such as getting or initializing the status of multiple elements.


## -struct-fields




### -field Element

A 
<a href="https://msdn.microsoft.com/96e9803b-16c4-415c-940a-f5df3edff3b3">CHANGER_ELEMENT</a> structure that represent the first element in the range.


### -field NumberOfElements

The number of elements in the range.


## -see-also




<a href="https://msdn.microsoft.com/96e9803b-16c4-415c-940a-f5df3edff3b3">CHANGER_ELEMENT</a>



<a href="https://msdn.microsoft.com/0745ee19-34f3-44c8-a52d-fb47448f0084">IOCTL_CHANGER_REINITIALIZE_TRANSPORT</a>
 

 

