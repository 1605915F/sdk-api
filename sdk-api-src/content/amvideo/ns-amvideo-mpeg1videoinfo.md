---
UID: NS:amvideo.tagMPEG1VIDEOINFO
title: MPEG1VIDEOINFO
author: windows-sdk-content
description: The MPEG1VIDEOINFO structure describes an MPEG-1 video stream.
old-location: dshow\mpeg1videoinfo.htm
tech.root: DirectShow
ms.assetid: ae5b8825-7c1c-4a44-b665-098732e6c3bc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MPEG1VIDEOINFO, MPEG1VIDEOINFO structure [DirectShow], MPEG1VIDEOINFOStructure, amvideo/MPEG1VIDEOINFO, dshow.mpeg1videoinfo, tagMPEG1VIDEOINFO
ms.topic: struct
req.header: amvideo.h
req.include-header: Dshow.h
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
 - amvideo.h
api_name:
 - MPEG1VIDEOINFO
product: Windows
targetos: Windows
req.typenames: MPEG1VIDEOINFO
req.redist: 
---

# MPEG1VIDEOINFO structure


## -description



The <b>MPEG1VIDEOINFO</b> structure describes an MPEG-1 video stream.




## -struct-fields




### -field hdr


<a href="https://msdn.microsoft.com/en-us/library/Dd407325(v=VS.85).aspx">VIDEOINFOHEADER</a> structure.


### -field dwStartTimeCode

25-bit group-of-pictures (GOP) time code at start of data.


### -field cbSequenceHeader

Length of the <b>bSequenceHeader</b> member, in bytes.


### -field bSequenceHeader

Start of an array that contains the sequence header, including quantization matrices, if any. The size of the array is given in the <b>cbSequenceHeader</b> member.


## -see-also




<a href="https://msdn.microsoft.com/378f6f43-5c05-4ae4-be24-956f9fc0cacf">DirectShow Structures</a>
 

 

