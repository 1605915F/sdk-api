---
UID: NF:amstream.IAMMediaStream.SetState
title: IAMMediaStream::SetState
author: windows-sdk-content
description: Note  This interface is deprecated. New applications should not use it. The SetState method sets the filter state.
old-location: dshow\iammediastream_setstate.htm
tech.root: DirectShow
ms.assetid: 2134c2cf-4d78-438c-8fb9-a96f87f682d9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAMMediaStream interface [DirectShow],SetState method, IAMMediaStream.SetState, IAMMediaStream::SetState, IAMMediaStreamSetState, SetState, SetState method [DirectShow], SetState method [DirectShow],IAMMediaStream interface, amstream/IAMMediaStream::SetState, dshow.iammediastream_setstate
ms.topic: method
req.header: amstream.h
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
 - COM
api_location:
 - amstream.h
api_name:
 - IAMMediaStream.SetState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMMediaStream::SetState


## -description



<div class="alert"><b>Note</b>  This interface is deprecated. New applications should not use it.</div>
<div> </div>
The <code>SetState</code> method sets the filter state.




## -parameters




### -param State [in]

Sets the filter's state, as specified by the <a href="https://msdn.microsoft.com/en-us/library/Dd375789(v=VS.85).aspx">FILTER_STATE</a> enumerated type.


## -returns



Returns S_OK if successful or E_INVALIDARG if the <i>State</i> parameter is invalid.




## -remarks



Applications should not call this method.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd319657(v=VS.85).aspx">IAMMediaStream Interface</a>
 

 

