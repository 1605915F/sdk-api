---
UID: NS:commoncontrols.tagIMAGELISTSTATS
title: IMAGELISTSTATS
author: windows-sdk-content
description: Contains image list statistics. Used by GetStatistics.
old-location: controls\IMAGELISTSTATS.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\imagelist\structures\imageliststats.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMAGELISTSTATS, IMAGELISTSTATS structure [Windows Controls], _shell_IMAGELISTSTATS, _shell_IMAGELISTSTATS_cpp, commoncontrols/IMAGELISTSTATS, controls.IMAGELISTSTATS, controls._shell_IMAGELISTSTATS
ms.topic: struct
req.header: commoncontrols.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Commoncontrols.idl
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
 - Commoncontrols.h
api_name:
 - IMAGELISTSTATS
product: Windows
targetos: Windows
req.typenames: IMAGELISTSTATS
req.redist: 
---

# IMAGELISTSTATS structure


## -description


Contains image list statistics. Used by <a href="https://msdn.microsoft.com/en-us/library/Bb761417(v=VS.85).aspx">GetStatistics</a>.


## -struct-fields




### -field cbSize

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

The image list size.


### -field cAlloc

Type: <b>int</b>

The number of images allocated.


### -field cUsed

Type: <b>int</b>

The number of images in use.


### -field cStandby

Type: <b>int</b>

The number of standby images.

