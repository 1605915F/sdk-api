---
UID: NS:windows.media.streaming.PositionInformation
title: PositionInformation
author: windows-sdk-content
description: Contains the current values of media playback position information obtained from the DMR.
old-location: mediastreaming\positioninformation.htm
tech.root: mediastreaming
ms.assetid: 9601c1ae-3fd2-4761-8aa7-102b72ef4733
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PositionInformation, PositionInformation structure [Media Streaming API], mediastreaming.positioninformation, windows/PositionInformation
ms.topic: struct
req.header: windows.media.streaming.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Windows.Media.Streaming.idl (reference Windows.Media.Streaming.idl)
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
 - windows.media.streaming.h
api_name:
 - PositionInformation
product: Windows
targetos: Windows
req.typenames: PositionInformation
req.redist: 
---

# PositionInformation structure


## -description


Contains the current values of media playback position information obtained from the DMR.


## -struct-fields




### -field streaming.PositionInformation.trackInformation

 


### -field streaming.PositionInformation.relativeTime

 




#### - relativeTime

The current playback position of the DMR.


#### - trackInformation

A <a href="https://msdn.microsoft.com/47398d9f-9462-49c1-a02c-985212a07363">TrackInformation</a> structure that contains the current track number and duration.

