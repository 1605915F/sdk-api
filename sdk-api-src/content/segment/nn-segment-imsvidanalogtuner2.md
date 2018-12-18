---
UID: NN:segment.IMSVidAnalogTuner2
title: IMSVidAnalogTuner2
author: windows-sdk-content
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later. The IMSVidAnalogTuner2 interface represents an analog-only tuner card that does not support the Broadcast Driver Architecture (BDA).
old-location: mstv\imsvidanalogtuner2.htm
tech.root: mstv
ms.assetid: 50d30a45-8cea-454c-b5d2-ff809b8a8206
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidAnalogTuner2, IMSVidAnalogTuner2 interface [Microsoft TV Technologies], IMSVidAnalogTuner2 interface [Microsoft TV Technologies],described, IMSVidAnalogTuner2Interface, mstv.imsvidanalogtuner2, segment/IMSVidAnalogTuner2
ms.topic: interface
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - IMSVidAnalogTuner2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidAnalogTuner2 interface


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        

The <b>IMSVidAnalogTuner2</b> interface represents an analog-only tuner card that does not support the Broadcast Driver Architecture (BDA).




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMSVidAnalogTuner2</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Dd694420(v=VS.85).aspx">IMSVidAnalogTuner</a>. <b>IMSVidAnalogTuner2</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMSVidAnalogTuner2</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694422(v=VS.85).aspx">get_NumAuxInputs</a>
</td>
<td align="left" width="63%">
The number of auxiliary inputs.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694423(v=VS.85).aspx">get_TunerModes</a>
</td>
<td align="left" width="63%">
Which tuner modes the tuner supports.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694424(v=VS.85).aspx">get_TVFormats</a>
</td>
<td align="left" width="63%">
Which TV formats the tuner supports.

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IMSVidAnalogTuner2)</code>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd694420(v=VS.85).aspx">IMSVidAnalogTuner</a>



<a href="https://msdn.microsoft.com/bf6c3ce9-1e56-4109-93f1-5b313e6ca19b">Video Control Interfaces</a>
 

 

