---
UID: NS:rectypes.tagCHARACTER_RANGE
title: CHARACTER_RANGE (rectypes.h)
author: windows-sdk-content
description: Specifies a range of Unicode points (characters).
old-location: tablet\character_range.htm
tech.root: tablet
ms.assetid: 51d13adf-170e-4172-b752-c9dac5a96fa5
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PCHARACTER_RANGE, 51d13adf-170e-4172-b752-c9dac5a96fa5, CHARACTER_RANGE, CHARACTER_RANGE structure [Tablet PC], rectypes/CHARACTER_RANGE, tablet.character_range"
ms.topic: struct
req.header: rectypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
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
 - rectypes.h
api_name:
 - CHARACTER_RANGE
product: Windows
targetos: Windows
req.typenames: CHARACTER_RANGE, *PCHARACTER_RANGE
req.redist: 
ms.custom: 19H1
---

# CHARACTER_RANGE structure


## -description



Specifies a range of Unicode points (characters).




## -struct-fields




### -field wcLow

 The low Unicode code point in the range of supported Unicode points.


### -field cChars

 The number of supported Unicode points in this range.


## -see-also




<a href="https://msdn.microsoft.com/047a72f9-a627-4c8b-b271-13d3c873abc9">GetEnabledUnicodeRanges Function</a>



<a href="https://msdn.microsoft.com/4a354073-e971-43ba-93c9-84fa2e8c59aa">GetUnicodeRanges Function</a>



<a href="https://msdn.microsoft.com/68c7c06b-eab1-419d-ad58-22cbd4c3065e">SetEnabledUnicodeRanges Function</a>
 

 

