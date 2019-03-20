---
UID: NS:hrtfapoapi.HrtfApoInit
title: HrtfApoInit (hrtfapoapi.h)
author: windows-sdk-content
description: Specifies parameters used to initialize HRTF spatial audio.
old-location: xaudio2\hrtfapoinit.htm
tech.root: xaudio2
ms.assetid: 686A2203-A991-427F-9D41-F3C679070127
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: HrtfApoInit, HrtfApoInit structure [XAudio2 Audio Mixing APIs], PHrtfApoInit, PHrtfApoInit structure pointer [XAudio2 Audio Mixing APIs], hrtfapoapi/HrtfApoInit, hrtfapoapi/PHrtfApoInit, xaudio2.hrtfapoinit
ms.topic: struct
req.header: hrtfapoapi.h
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
 - HrtfApoApi.h
api_name:
 - HrtfApoInit
product: Windows
targetos: Windows
req.typenames: HrtfApoInit
req.redist: 
---

# HrtfApoInit structure


## -description


Specifies parameters used to initialize HRTF spatial audio.


## -struct-fields




### -field distanceDecay

The decay type. If you pass in nullptr, the default value is used. The default is natural decay.


### -field directivity

The directivity type. If you pass in nullptr, the default value is used. The default directivity is omni-directional.


## -see-also




<a href="https://msdn.microsoft.com/24E3CD0D-FC0D-4B1B-961F-BE48935F7B71">CreateHrtfApo</a>



<a href="https://msdn.microsoft.com/3656aaf9-7a3a-2a5b-50f5-d279ce8a9e6c">Structures</a>
 

 

