---
UID: NS:medparam._MP_ENVELOPE_SEGMENT
title: MP_ENVELOPE_SEGMENT
author: windows-sdk-content
description: The MP_ENVELOPE_SEGMENT structure defines an envelope segment used by an envelope-following parameter.
old-location: dshow\mp_envelope_segment.htm
tech.root: DirectShow
ms.assetid: b7386b63-c563-42dd-851c-780bf1043f65
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MPF_ENVLP_BEGIN_CURRENTVAL, MPF_ENVLP_BEGIN_NEUTRALVAL, MPF_ENVLP_STANDARD, MP_ENVELOPEStructure, MP_ENVELOPE_SEGMENT, MP_ENVELOPE_SEGMENT structure [DirectShow], dshow.mp_envelope_segment, medparam/MP_ENVELOPE_SEGMENT
ms.topic: struct
req.header: medparam.h
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
 - HeaderDef
api_location:
 - Medparam.h
api_name:
 - MP_ENVELOPE_SEGMENT
product: Windows
targetos: Windows
req.typenames: MP_ENVELOPE_SEGMENT
req.redist: 
---

# MP_ENVELOPE_SEGMENT structure


## -description



The <code>MP_ENVELOPE_SEGMENT</code> structure defines an envelope segment used by an envelope-following parameter.




## -struct-fields




### -field rtStart

Start time of the segment, relative to the time stamp on the first buffer, in 100-nanosecond units.


### -field rtEnd

Stop time of the segment, relative to the time stamp on the first buffer, in 100-nanosecond units.


### -field valStart

Initial value of the parameter, at the start of the segment.


### -field valEnd

Final value of the parameter, at the end of the segment.


### -field iCurve

Member of the <b>MP_CURVE_TYPE</b> enumerated type that specifies the curve followed by the parameter.


### -field flags

Specifies one of the following flags.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="MPF_ENVLP_STANDARD"></a><a id="mpf_envlp_standard"></a><dl>
<dt><b>MPF_ENVLP_STANDARD</b></dt>
<dt>0x0000</dt>
</dl>
</td>
<td width="60%">
Use all the information provided with the envelope segment.

</td>
</tr>
<tr>
<td width="40%"><a id="MPF_ENVLP_BEGIN_CURRENTVAL"></a><a id="mpf_envlp_begin_currentval"></a><dl>
<dt><b>MPF_ENVLP_BEGIN_CURRENTVAL</b></dt>
<dt>0x0001</dt>
</dl>
</td>
<td width="60%">
Ignore the specified start value. Start from the current value.

</td>
</tr>
<tr>
<td width="40%"><a id="MPF_ENVLP_BEGIN_NEUTRALVAL"></a><a id="mpf_envlp_begin_neutralval"></a><dl>
<dt><b>MPF_ENVLP_BEGIN_NEUTRALVAL</b></dt>
<dt>0x0002</dt>
</dl>
</td>
<td width="60%">
Ignore the specified start value. Start from the neutral value. (See <a href="https://msdn.microsoft.com/en-us/library/Dd390745(v=VS.85).aspx">MP_PARAMINFO</a>.)

</td>
</tr>
</table>
 


## -see-also




<a href="https://msdn.microsoft.com/82c8ea74-1c5e-4370-9075-6db2ed6b2c91">DMO Structures</a>
 

 

