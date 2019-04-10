---
UID: NF:segment.IMSVidPlayback.put_Rate
title: IMSVidPlayback::put_Rate (segment.h)
author: windows-sdk-content
description: The put_Rate method sets the playback rate.
old-location: mstv\imsvidplayback_put_rate.htm
tech.root: mstv
ms.assetid: a3542d7c-6333-4832-a24a-0b778ea83a4c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IMSVidPlayback interface [Microsoft TV Technologies],put_Rate method, IMSVidPlayback.put_Rate, IMSVidPlayback::put_Rate, IMSVidPlaybackput_Rate, mstv.imsvidplayback_put_rate, put_Rate, put_Rate method [Microsoft TV Technologies], put_Rate method [Microsoft TV Technologies],IMSVidPlayback interface, segment/IMSVidPlayback::put_Rate
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
 - IMSVidPlayback.put_Rate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidPlayback::put_Rate


## -description


The <b>put_Rate</b> method sets the playback rate.


## -parameters




### -param plRate [in]

Specifies the playback rate, as a ratio to the authored rate. For example, 0.5 means half the normal speed, 1.0 means normal speed, and 2.0 means twice the normal speed.


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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The source filter does not support the specified rate.

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



Call the <a href="https://msdn.microsoft.com/49f78dd8-f26e-456d-b67e-155ae0ed5419">IMSVidCtl::Build</a> or <a href="https://msdn.microsoft.com/ec0e2a88-13c0-42f3-ba7d-8ebff1234b86">IMSVidCtl::View</a> method before calling this method.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd694586(v=VS.85).aspx">IMSVidPlayback Interface</a>
 

 

