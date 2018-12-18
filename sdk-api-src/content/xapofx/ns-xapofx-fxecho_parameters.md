---
UID: NS:xapofx.FXECHO_PARAMETERS
title: FXECHO_PARAMETERS
author: windows-sdk-content
description: Parameters for use with the FXECHO XAPOFX.
old-location: xaudio2\fxecho_parameters.htm
tech.root: xaudio2
ms.assetid: T:Microsoft.directx_sdk.xapofx.FXECHO_PARAMETERS
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FXECHO_PARAMETERS, FXECHO_PARAMETERS structure [XAudio2 Audio Mixing APIs], xapofx/FXECHO_PARAMETERS, xaudio2.fxecho_parameters
ms.topic: struct
req.header: xapofx.h
req.include-header: 
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
 - xapofx.h
api_name:
 - FXECHO_PARAMETERS
product: Windows
targetos: Windows
req.typenames: FXECHO_PARAMETERS
req.redist: 
---

# FXECHO_PARAMETERS structure


## -description


Parameters for use with the <a href="https://msdn.microsoft.com/762062de-4e19-5e42-8059-e2f8741bd362">FXECHO XAPOFX</a>.


## -struct-fields




### -field WetDryMix

Ratio of wet (processed) signal to dry (original) signal.


### -field Feedback

Amount of output to feed back into input.


### -field Delay

Delay to all channels in milliseconds. This value must be between <b>FXECHO_MIN_DELAY</b> and <a href="https://msdn.microsoft.com/en-us/library/Hh405045(v=VS.85).aspx">FXECHO_INITDATA</a>.<b>MaxDelay</b>.


## -remarks



Echo only supports FLOAT32 audio formats.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Windows 10 (XAudio2.9); Windows 8, Windows Phone 8 (XAudio 2.8); DirectX SDK (XAudio 2.7)




## -see-also




<a href="https://msdn.microsoft.com/3656aaf9-7a3a-2a5b-50f5-d279ce8a9e6c">Structures</a>
 

 

