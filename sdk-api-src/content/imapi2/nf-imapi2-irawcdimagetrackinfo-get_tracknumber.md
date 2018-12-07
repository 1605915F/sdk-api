---
UID: NF:imapi2.IRawCDImageTrackInfo.get_TrackNumber
title: IRawCDImageTrackInfo::get_TrackNumber
author: windows-sdk-content
description: Retrieves the track number for this track.
old-location: imapi\irawcdimagetrackinfo_get_tracknumber.htm
tech.root: imapi
ms.assetid: ccc84237-3819-45b4-980a-a73669f605fb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IRawCDImageTrackInfo interface [IMAPI],get_TrackNumber method, IRawCDImageTrackInfo.get_TrackNumber, IRawCDImageTrackInfo::get_TrackNumber, get_TrackNumber, get_TrackNumber method [IMAPI], get_TrackNumber method [IMAPI],IRawCDImageTrackInfo interface, imapi.irawcdimagetrackinfo_get_tracknumber, imapi2/IRawCDImageTrackInfo::get_TrackNumber
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: imapi2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2.idl
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
 - COM
api_location:
 - imapi2.h
api_name:
 - IRawCDImageTrackInfo.get_TrackNumber
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRawCDImageTrackInfo::get_TrackNumber


## -description


Retrieves the track number for this track.


## -parameters




### -param value [out]

The track number for this track.


## -returns



S_OK is returned on success, but other success codes may be returned as a result of implementation.




## -remarks



While this value is often identical to the <b>TrackIndex</b> property, it is possible for pure audio discs to start with a track other than track number 1.  This means that the more general formula is that this value is ( TrackIndex + FirstTrackNumber - 1).

This method is supported in Windows Server 2003 with Service Pack 1 (SP1), Windows XP with Service Pack 2 (SP2),  and Windows Vista  via the <a href="http://go.microsoft.com/fwlink/p/?linkid=141659">Windows Feature Pack for Storage</a>. All  features provided by this  update package are supported natively in Windows 7 and Windows Server 2008 R2.




## -see-also




<a href="https://msdn.microsoft.com/5d074279-35fb-48d0-b298-c1a83f57d805">IRawCDImageTrackInfo</a>
 

 

