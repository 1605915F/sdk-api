---
UID: NF:segment.IMSVidPlayback.Step
title: IMSVidPlayback::Step (segment.h)
author: windows-sdk-content
description: The Step method steps through the video stream by a specified number of frames.
old-location: mstv\imsvidplayback_step.htm
tech.root: mstv
ms.assetid: 8e971571-61f4-4b24-81a7-45fa17b6b785
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidPlayback interface [Microsoft TV Technologies],Step method, IMSVidPlayback.Step, IMSVidPlayback::Step, IMSVidPlaybackStep, Step, Step method [Microsoft TV Technologies], Step method [Microsoft TV Technologies],IMSVidPlayback interface, mstv.imsvidplayback_step, segment/IMSVidPlayback::Step
ms.topic: method
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Segment.idl
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
 - segment.h
api_name:
 - IMSVidPlayback.Step
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidPlayback::Step


## -description


The <b>Step</b> method steps through the video stream by a specified number of frames.


## -parameters




### -param lStep [in]

Specifies how many frames to step. If <i>lStep</i> is 1, the Video Control steps forward one frame. If <i>lStep</i> is a number <i>N</i> greater than 1, the Video Control skips <i>N</i> - 1 frames and shows the <i>N</i>th frame.


## -returns



The method returns an <b>HRESULT</b>. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
Not implemented.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_STATE</b></dt>
</dl>
</td>
<td width="60%">
The graph is not built. Call the <a href="https://msdn.microsoft.com/49f78dd8-f26e-456d-b67e-155ae0ed5419">Build</a> or <a href="https://msdn.microsoft.com/ec0e2a88-13c0-42f3-ba7d-8ebff1234b86">View</a> method on the Video Control.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 

<div class="alert"><b>Note</b>  The value ERROR_INVALID_STATE is converted to an <b>HRESULT</b> with the <b>HRESULT_FROM_WIN32</b> macro.</div>
<div> </div>



## -remarks



Although a negative value for <i>lStep</i> is defined as stepping backward, that functionality is currently not implemented, and the method returns E_NOTIMPL.

Call the <a href="https://msdn.microsoft.com/49f78dd8-f26e-456d-b67e-155ae0ed5419">IMSVidCtl::Build</a> or <a href="https://msdn.microsoft.com/ec0e2a88-13c0-42f3-ba7d-8ebff1234b86">IMSVidCtl::View</a> method before calling this method.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd694586(v=VS.85).aspx">IMSVidPlayback Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd694589(v=VS.85).aspx">IMSVidPlayback::get_CanStep</a>
 

 

