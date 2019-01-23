---
UID: NF:amvideo.BITMASKS
title: BITMASKS macro
author: windows-sdk-content
description: The BITMASKS macro retrieves the color masks from a VIDEOINFO structure.
old-location: dshow\bitmasks.htm
tech.root: DirectShow
ms.assetid: e90ddeab-a3d6-4d34-8608-4d8831d81fe5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BITMASKS, BITMASKS macro [DirectShow], amvideo/BITMASKS, dshow.bitmasks
ms.topic: macro
req.header: amvideo.h
req.include-header: Streams.h
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
 - Amvideo.h
api_name:
 - BITMASKS
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# BITMASKS macro


## -description


The <code>BITMASKS</code> macro retrieves the color masks from a <a href="https://msdn.microsoft.com/en-us/library/Dd407323(v=VS.85).aspx">VIDEOINFO</a> structure.


## -parameters




### -param pbmi

Pointer to a <a href="https://msdn.microsoft.com/en-us/library/Dd407323(v=VS.85).aspx">VIDEOINFO</a> structure.


## -remarks



This macro calculates the address as an offset from the start of the <a href="https://msdn.microsoft.com/153c08a8-d32c-4e9d-9da9-b915eb172327">BITMAPINFOHEADER</a> structure, using the value of <b>bmiHeader.biSize</b>. Make sure to initialize the <a href="https://msdn.microsoft.com/en-us/library/Dd407323(v=VS.85).aspx">VIDEOINFO</a> structure before calling this macro.

You can access the color masks in the array using the following constants, defined in Amvideo.h:

<pre class="syntax" xml:space="preserve"><code>#define iRED   0
#define iGREEN 1
#define iBLUE  2  </code></pre>

#### Examples


```
VIDEOINFO *pVi;

/* Initialize pVi (not shown). */

DWORD dwRed   = BITMASKS(pVi)[iRED];
DWORD dwGreen = BITMASKS(pVi)[iGREEN]; 
DWORD dwBlue  = BITMASKS(pVi)[iBLUE];
```





## -see-also




<a href="https://msdn.microsoft.com/02401edc-362b-4f6c-b10b-c46b30b3ebe7">Video and Image Functions</a>
 

 

