---
UID: NF:evr.IMFVideoMixerControl.GetStreamOutputRect
title: IMFVideoMixerControl::GetStreamOutputRect (evr.h)
author: windows-sdk-content
description: Retrieves the position of a video stream within the composition rectangle.
old-location: mf\imfvideomixercontrol_getstreamoutputrect.htm
tech.root: medfound
ms.assetid: 6de631cd-f85e-4f53-b14c-8ca3cd65b719
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 6de631cd-f85e-4f53-b14c-8ca3cd65b719, GetStreamOutputRect, GetStreamOutputRect method [Media Foundation], GetStreamOutputRect method [Media Foundation],IMFVideoMixerControl interface, IMFVideoMixerControl interface [Media Foundation],GetStreamOutputRect method, IMFVideoMixerControl.GetStreamOutputRect, IMFVideoMixerControl::GetStreamOutputRect, evr/IMFVideoMixerControl::GetStreamOutputRect, mf.imfvideomixercontrol_getstreamoutputrect
ms.topic: method
req.header: evr.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - strmiids.lib
 - strmiids.dll
api_name:
 - IMFVideoMixerControl.GetStreamOutputRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFVideoMixerControl::GetStreamOutputRect


## -description



Retrieves the position of a video stream within the composition rectangle.




## -parameters




### -param dwStreamID [in]

The identifier of the stream. For the EVR media sink, the stream identifier is defined when the <a href="https://msdn.microsoft.com/1b05ef87-5559-4310-942c-54ab113eb42d">IMFMediaSink::AddStreamSink</a> method is called. For the DirectShow EVR filter, the stream identifier corresponds to the pin index. The reference stream is always stream 0.


### -param pnrcOutput [out]

Pointer to an <a href="https://msdn.microsoft.com/c1dd42ca-64a0-4f30-82e1-eda3f4721526">MFVideoNormalizedRect</a> structure that receives the bounding rectangle, in normalized coordinates.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
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
<tr>
<td width="40%">
<dl>
<dt><b>MF_E_INVALIDSTREAMNUMBER</b></dt>
</dl>
</td>
<td width="60%">
Invalid stream identifier.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/1c985558-d25d-4f51-978a-58c05943dab9">Enhanced Video Renderer</a>



<a href="https://msdn.microsoft.com/8b5f54e3-c6da-4201-857a-9c718ad911db">IMFVideoMixerControl</a>
 

 

