---
UID: NS:ddrawint._DD_MAPMEMORYDATA
title: DD_MAPMEMORYDATA (ddrawint.h)
author: windows-sdk-content
description: The DD_MAPMEMORYDATA structure contains the information necessary to map or unmap a frame buffer into user-mode memory.
old-location: display\dd_mapmemorydata.htm
tech.root: display
ms.assetid: 51d8b35f-883c-4e47-a0e6-af6c8ade8e54
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDD_MAPMEMORYDATA, DD_MAPMEMORYDATA, DD_MAPMEMORYDATA structure [Display Devices], ddrawint/DD_MAPMEMORYDATA, ddstrcts_8ed973e1-2324-4dba-bcff-78442d5f33ee.xml, display.dd_mapmemorydata"
ms.topic: struct
req.header: ddrawint.h
req.include-header: Winddi.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - ddrawint.h
api_name:
 - DD_MAPMEMORYDATA
product: Windows
targetos: Windows
req.typenames: "*PDD_MAPMEMORYDATA, DD_MAPMEMORYDATA"
req.redist: 
ms.custom: 19H1
---

# DD_MAPMEMORYDATA structure


## -description


The DD_MAPMEMORYDATA structure contains the information necessary to map or unmap a frame buffer into user-mode memory.


## -struct-fields




### -field lpDD

Points to a <a href="https://msdn.microsoft.com/a59f064b-48cf-4491-82cd-84f59467af87">DD_DIRECTDRAW_GLOBAL</a> structure that describes the driver's device.


### -field bMap

Specifies the memory operation that the driver should perform. A value of <b>TRUE</b> indicates that the driver should map memory; <b>FALSE</b> means that the driver should unmap memory.


### -field hProcess

Handle to the process whose address space is affected.


### -field fpProcess

Specifies the location in which the driver should return the base address of the process's memory-mapped space when <b>bMap</b> is <b>TRUE</b>. When <b>bMap</b> is <b>FALSE</b>, <b>fpProcess</b> contains the base address of the memory to be unmapped by the driver.


### -field ddRVal

Specifies the location in which the driver writes the return value of the <a href="https://msdn.microsoft.com/a05e2ba8-dfe1-447d-acfa-0eb8f4252107">DdMapMemory</a> callback. A return code of DD_OK indicates success. For more information, see <a href="https://msdn.microsoft.com/da4cc7d7-6826-48aa-96c6-004e31fc3e3e">Return Values for DirectDraw</a>.


## -see-also




<a href="https://msdn.microsoft.com/a05e2ba8-dfe1-447d-acfa-0eb8f4252107">DdMapMemory</a>
 

 

