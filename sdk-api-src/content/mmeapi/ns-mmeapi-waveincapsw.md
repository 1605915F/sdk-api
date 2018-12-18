---
UID: NS:mmeapi.tagWAVEINCAPSW
title: WAVEINCAPSW
author: windows-sdk-content
description: The WAVEINCAPS structure describes the capabilities of a waveform-audio input device.
old-location: multimedia\waveincaps.htm
tech.root: Multimedia
ms.assetid: e96524fd-82d3-4363-989b-23fb20786f3c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPWAVEINCAPSW, *NPWAVEINCAPSW, *PWAVEINCAPSW, WAVEINCAPS, WAVEINCAPS structure [Windows Multimedia], WAVEINCAPSW, _win32_WAVEINCAPS_str, mmeapi/WAVEINCAPS, multimedia.waveincaps, tagWAVEINCAPSA, tagWAVEINCAPSW, waveincaps_tag"
ms.topic: struct
req.header: mmeapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - mmeapi.h
api_name:
 - WAVEINCAPS
product: Windows
targetos: Windows
req.typenames: WAVEINCAPSW, *PWAVEINCAPSW, *NPWAVEINCAPSW, *LPWAVEINCAPSW
req.redist: 
---

# WAVEINCAPSW structure


## -description



The <b>WAVEINCAPS</b> structure describes the capabilities of a waveform-audio input device.




## -struct-fields




### -field wMid

Manufacturer identifier for the device driver for the waveform-audio input device. Manufacturer identifiers are defined in <a href="https://msdn.microsoft.com/ab68ffd2-208f-445b-9f5c-37159edb4d4b">Manufacturer and Product Identifiers</a>.


### -field wPid

Product identifier for the waveform-audio input device. Product identifiers are defined in <a href="https://msdn.microsoft.com/ab68ffd2-208f-445b-9f5c-37159edb4d4b">Manufacturer and Product Identifiers</a>.


### -field vDriverVersion

Version number of the device driver for the waveform-audio input device. The high-order byte is the major version number, and the low-order byte is the minor version number.


### -field szPname

Product name in a null-terminated string.


### -field dwFormats

Standard formats that are supported. Can be a combination of the following:

<table>
<tr>
<th>Format</th>
<th>Description</th>
</tr>
<tr>
<td>WAVE_FORMAT_1M08</td>
<td>11.025 kHz, mono, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_1M16</td>
<td>11.025 kHz, mono, 16-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_1S08</td>
<td>11.025 kHz, stereo, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_1S16</td>
<td>11.025 kHz, stereo, 16-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_2M08</td>
<td>22.05 kHz, mono, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_2M16</td>
<td>22.05 kHz, mono, 16-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_2S08</td>
<td>22.05 kHz, stereo, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_2S16</td>
<td>22.05 kHz, stereo, 16-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_4M08</td>
<td>44.1 kHz, mono, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_4M16</td>
<td>44.1 kHz, mono, 16-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_4S08</td>
<td>44.1 kHz, stereo, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_4S16</td>
<td>44.1 kHz, stereo, 16-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_96M08</td>
<td>96 kHz, mono, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_96M16</td>
<td>96 kHz, mono, 16-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_96S08</td>
<td>96 kHz, stereo, 8-bit</td>
</tr>
<tr>
<td>WAVE_FORMAT_96S16</td>
<td>96 kHz, stereo, 16-bit</td>
</tr>
</table>
 


### -field wChannels

Number specifying whether the device supports mono (1) or stereo (2) input.


#### - wReserved1

Padding.


## -see-also




<a href="https://msdn.microsoft.com/3188355c-65be-4372-8e87-e7f755982592">Waveform Audio</a>



<a href="https://msdn.microsoft.com/4ae84ba8-f444-4d9e-adc8-343b4ee764cc">Waveform Structures</a>
 

 

