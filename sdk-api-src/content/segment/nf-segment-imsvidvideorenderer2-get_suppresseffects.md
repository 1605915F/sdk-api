---
UID: NF:segment.IMSVidVideoRenderer2.get_SuppressEffects
title: IMSVidVideoRenderer2::get_SuppressEffects
author: windows-sdk-content
description: The get_SuppressEffects method retrieves settings that control power management and visual effects.
old-location: mstv\imsvidvideorenderer2_get_suppresseffects.htm
tech.root: mstv
ms.assetid: 5a8546f8-61de-4e98-bee3-26ca4d0ea2e4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidVideoRenderer2 interface [Microsoft TV Technologies],get_SuppressEffects method, IMSVidVideoRenderer2.get_SuppressEffects, IMSVidVideoRenderer2::get_SuppressEffects, IMSVidVideoRenderer2get_SuppressEffects, get_SuppressEffects, get_SuppressEffects method [Microsoft TV Technologies], get_SuppressEffects method [Microsoft TV Technologies],IMSVidVideoRenderer2 interface, mstv.imsvidvideorenderer2_get_suppresseffects, segment/IMSVidVideoRenderer2::get_SuppressEffects
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
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
 - IMSVidVideoRenderer2.get_SuppressEffects
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidVideoRenderer2::get_SuppressEffects


## -description


The <b>get_SuppressEffects</b> method retrieves settings that control power management and visual effects.


## -parameters




### -param bSuppress [out]

Receives the value VARIANT_TRUE or VARIANT_FALSE. For more information, see <a href="https://msdn.microsoft.com/d362addb-626a-42f8-9b95-82189a338527">IMSVidVideoRenderer2::put_SuppressEffects</a>.


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
NULL pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/caaa2cf1-15be-47dc-82db-06915a55ba03">IMSVidVideoRenderer2 Interface</a>
 

 

