---
UID: NS:dxvahd._DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA
title: DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA (dxvahd.h)
author: windows-sdk-content
description: Specifies the destination rectangle for an input stream, when using Microsoft DirectX Video Acceleration High Definition (DXVA-HD).
old-location: mf\dxvahd_stream_state_destination_rect_data.htm
tech.root: medfound
ms.assetid: f850531b-eee0-4943-8c41-050ec78eab63
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA, DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA structure [Media Foundation], FALSE, TRUE, dxvahd/DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA, mf.dxvahd_stream_state_destination_rect_data
ms.topic: struct
req.header: dxvahd.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - dxvahd.h
api_name:
 - DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA
product: Windows
targetos: Windows
req.typenames: DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA
req.redist: 
ms.custom: 19H1
---

# DXVAHD_STREAM_STATE_DESTINATION_RECT_DATA structure


## -description


Specifies the destination rectangle for an input stream, when using Microsoft DirectX Video Acceleration High Definition (DXVA-HD).


## -struct-fields




### -field Enable

Specifies whether to use the destination rectangle, or use the entire output surface. The default state value is <b>FALSE</b>.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="TRUE"></a><a id="true"></a><dl>
<dt><b>TRUE</b></dt>
</dl>
</td>
<td width="60%">
Use the destination rectangle given in the <b>DestinationRect</b> member.

</td>
</tr>
<tr>
<td width="40%"><a id="FALSE"></a><a id="false"></a><dl>
<dt><b>FALSE</b></dt>
</dl>
</td>
<td width="60%">
Use the entire output surface as the destination rectangle.

</td>
</tr>
</table>
 


### -field DestinationRect

The <i>destination rectangle</i>, which defines the portion of the output surface where the source rectangle is blitted. The destination rectangle is given in pixel coordinates, relative to the output surface. The default value is an empty rectangle, (0, 0, 0, 0).

If the <b>Enable</b> member is <b>FALSE</b>, the <b>DestinationRect</b> member is ignored.


## -see-also




<a href="https://msdn.microsoft.com/38ebec28-c4fc-4e72-ac87-1e41707d1908">DXVA-HD</a>



<a href="https://msdn.microsoft.com/75036101-7498-4d66-afc3-df76ae3cca39">DXVAHD_STREAM_STATE</a>



<a href="https://msdn.microsoft.com/584c087e-53f0-42d8-99ed-a0d013379363">Direct3D Video Structures</a>



<a href="https://msdn.microsoft.com/40a8444f-576e-40ff-804e-0912812f0ee6">IDXVAHD_VideoProcessor::SetVideoProcessStreamState</a>



<a href="https://msdn.microsoft.com/39fdd724-13ca-48ab-8a55-93529d1da3b4">Media Foundation Structures</a>
 

 

