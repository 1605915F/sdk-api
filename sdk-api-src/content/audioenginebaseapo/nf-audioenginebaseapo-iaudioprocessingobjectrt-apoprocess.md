---
UID: NF:audioenginebaseapo.IAudioProcessingObjectRT.APOProcess
title: IAudioProcessingObjectRT::APOProcess
author: windows-sdk-content
description: The APOProcess method causes the APO to make a processing pass.
old-location: audio\iaudioprocessingobjectrt_apoprocess.htm
tech.root: audio
ms.assetid: b32f3cc9-3ac0-47ff-a428-f0476bd1f39e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: APOProcess, APOProcess method [Audio Devices], APOProcess method [Audio Devices],IAudioProcessingObjectRT interface, IAudioProcessingObjectRT interface [Audio Devices],APOProcess method, IAudioProcessingObjectRT.APOProcess, IAudioProcessingObjectRT::APOProcess, audio.iaudioprocessingobjectrt_apoprocess, audio_syseffects_r_7ef87c04-2fe2-46b9-9c4a-0e604639132c.xml, audioenginebaseapo/IAudioProcessingObjectRT::APOProcess
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: audioenginebaseapo.h
req.include-header: 
req.target-type: Universal
req.target-min-winverclnt: Available with Windows Vista and later versions of the Windows operating system.
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
req.lib: Audioenginebaseapo.idl
req.dll: 
req.irql: All levels
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Audioenginebaseapo.idl
 - Audioenginebaseapo.idl.dll
api_name:
 - IAudioProcessingObjectRT.APOProcess
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAudioProcessingObjectRT::APOProcess


## -description


The APOProcess method causes the APO to make a processing pass.


## -parameters




### -param u32NumInputConnections [in]

The number of input connections that are attached to this APO.


### -param ppInputConnections [in]

An array of input connection property structures. There is one structure per input connection.


### -param u32NumOutputConnections [in]

The number of output connections that are attached to this APO.


### -param ppOutputConnections [in, out]

An array of output connection property structures. There is one structure per output connection.


## -returns



None

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
</table>
 




## -remarks



The <code>APOProcess</code> method must not change the data in the ppOutputConnections array. But it must set the properties of the output connections after processing.

The <code>APOProcess</code> method is called from a real-time processing thread. The implementation of this method must not touch paged memory and it should not call any system blocking routines.

For a detailed look at an implementation of this method, see the <a href="https://msdn.microsoft.com/bafbc56c-53a3-41a5-b077-3289967daf87">Swap sample code</a> and refer to the Swapapolfx.cpp file.




## -see-also




<a href="https://msdn.microsoft.com/bafbc56c-53a3-41a5-b077-3289967daf87">Swap sample code</a>
 

 

