---
UID: NF:mmeapi.mixerGetLineControlsA
title: mixerGetLineControlsA function (mmeapi.h)
author: windows-sdk-content
description: The mixerGetLineControls function retrieves one or more controls associated with an audio line.
old-location: multimedia\mixergetlinecontrols.htm
tech.root: Multimedia
ms.assetid: 48fa3396-f3ec-411a-9ea7-d7e82d606f14
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "_win32_mixerGetLineControls, mixerGetLineControls, mixerGetLineControls function [Windows Multimedia], mixerGetLineControlsA, mixerGetLineControlsW, mmeapi/mixerGetLineControls, mmeapi/mixerGetLineControlsA, mmeapi/mixerGetLineControlsW, multimedia.mixergetlinecontrols"
ms.topic: function
req.header: mmeapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: mixerGetLineControlsW (Unicode) and mixerGetLineControlsA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Winmm.lib
req.dll: Winmm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Winmm.dll
 - API-MS-Win-mm-mme-l1-1-0.dll
 - winmmbase.dll
api_name:
 - mixerGetLineControls
 - mixerGetLineControlsA
 - mixerGetLineControlsW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# mixerGetLineControlsA function


## -description



The <b>mixerGetLineControls</b> function retrieves one or more controls associated with an audio line.




## -parameters




### -param hmxobj

Handle to the mixer device object that is being queried.


### -param pmxlc

Pointer to a <a href="https://msdn.microsoft.com/a028785b-2d58-41da-825b-32e98fb44405">MIXERLINECONTROLS</a> structure. This structure is used to reference one or more <a href="https://msdn.microsoft.com/2ddbcf82-9204-43c6-8235-8bce6a55bb36">MIXERCONTROL</a> structures to be filled with information about the controls associated with an audio line. The <b>cbStruct</b> member of the <b>MIXERLINECONTROLS</b> structure must always be initialized to be the size, in bytes, of the <b>MIXERLINECONTROLS</b> structure.


### -param fdwControls

Flags for retrieving information about one or more controls associated with an audio line. The following values are defined.

<table>
<tr>
<th>Value
</th>
<th>Meaning
</th>
</tr>
<tr>
<td>MIXER_GETLINECONTROLSF_ALL</td>
<td>The <i>pmxlc</i> parameter references a list of <a href="https://msdn.microsoft.com/2ddbcf82-9204-43c6-8235-8bce6a55bb36">MIXERCONTROL</a> structures that will receive information on all controls associated with the audio line identified by the <b>dwLineID</b> member of the <a href="https://msdn.microsoft.com/a028785b-2d58-41da-825b-32e98fb44405">MIXERLINECONTROLS</a> structure. The <b>cControls</b> member must be initialized to the number of controls associated with the line. This number is retrieved from the <b>cControls</b> member of the <a href="https://msdn.microsoft.com/a314cdcd-dd52-49f1-92b4-c8e3775dcbe2">MIXERLINE</a> structure returned by the <a href="https://msdn.microsoft.com/125f09a6-df7f-4aa0-9180-410025b617e2">mixerGetLineInfo</a> function. The <b>cbmxctrl</b> member must be initialized to the size, in bytes, of a single <b>MIXERCONTROL</b> structure. The <b>pamxctrl</b> member must point to the first <b>MIXERCONTROL</b> structure to be filled. The <b>dwControlID</b> and <b>dwControlType</b> members are ignored for this query.</td>
</tr>
<tr>
<td>MIXER_GETLINECONTROLSF_ONEBYID</td>
<td>The <i>pmxlc</i> parameter references a single <a href="https://msdn.microsoft.com/2ddbcf82-9204-43c6-8235-8bce6a55bb36">MIXERCONTROL</a> structure that will receive information on the control identified by the <b>dwControlID</b> member of the <a href="https://msdn.microsoft.com/a028785b-2d58-41da-825b-32e98fb44405">MIXERLINECONTROLS</a> structure. The <b>cControls</b> member must be initialized to 1. The <b>cbmxctrl</b> member must be initialized to the size, in bytes, of a single <b>MIXERCONTROL</b> structure. The <b>pamxctrl</b> member must point to a <b>MIXERCONTROL</b> structure to be filled. The <b>dwLineID</b> and <b>dwControlType</b> members are ignored for this query. This query is usually used to refresh a control after receiving a <a href="https://msdn.microsoft.com/921c55a7-86c0-43d1-b817-bfbd3c4bb28b">MM_MIXM_CONTROL_CHANGE</a> control change notification message by the user-defined callback (see <a href="https://msdn.microsoft.com/7977680b-0967-4b85-9926-fc2725681de9">mixerOpen</a>).</td>
</tr>
<tr>
<td>MIXER_GETLINECONTROLSF_ONEBYTYPE</td>
<td>The <b>mixerGetLineControls</b> function retrieves information about the first control of a specific class for the audio line that is being queried. The <i>pmxlc</i> parameter references a single <a href="https://msdn.microsoft.com/2ddbcf82-9204-43c6-8235-8bce6a55bb36">MIXERCONTROL</a> structure that will receive information about the specific control. The audio line is identified by the <b>dwLineID</b> member. The control class is specified in the <b>dwControlType</b> member of the <a href="https://msdn.microsoft.com/a028785b-2d58-41da-825b-32e98fb44405">MIXERLINECONTROLS</a> structure.The <b>dwControlID</b> member is ignored for this query. This query can be used by an application to get information on a single control associated with a line. For example, you might want your application to use a peak meter only from a waveform-audio output line.

</td>
</tr>
<tr>
<td>MIXER_OBJECTF_AUX</td>
<td>The <i>hmxobj</i> parameter is an auxiliary device identifier in the range of zero to one less than the number of devices returned by the <a href="https://msdn.microsoft.com/6e36d549-83ba-4a67-b9d7-047e7d3a5613">auxGetNumDevs</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_HMIDIIN</td>
<td>The <i>hmxobj</i> parameter is the handle of a MIDI input device. This handle must have been returned by the <a href="https://msdn.microsoft.com/230deaef-9473-426f-a0eb-14e259600e68">midiInOpen</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_HMIDIOUT</td>
<td>The <i>hmxobj</i> parameter is the handle of a MIDI output device. This handle must have been returned by the <a href="https://msdn.microsoft.com/929cd4d1-6912-4456-a6c7-24a819799e46">midiOutOpen</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_HMIXER</td>
<td>The <i>hmxobj</i> parameter is a mixer device handle returned by the <a href="https://msdn.microsoft.com/7977680b-0967-4b85-9926-fc2725681de9">mixerOpen</a> function. This flag is optional.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_HWAVEIN</td>
<td>The <i>hmxobj</i> parameter is a waveform-audio input handle returned by the <a href="https://msdn.microsoft.com/41b5b581-d35c-48ad-adcf-659126c4af50">waveInOpen</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_HWAVEOUT</td>
<td>The <i>hmxobj</i> parameter is a waveform-audio output handle returned by the <a href="https://msdn.microsoft.com/ef02221b-df45-4fc3-8d9d-f119fa802d34">waveOutOpen</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_MIDIIN</td>
<td>The <i>hmxobj</i> parameter is the identifier of a MIDI input device. This identifier must be in the range of zero to one less than the number of devices returned by the <a href="https://msdn.microsoft.com/23303bb2-e053-4a19-a63a-4e017b861af6">midiInGetNumDevs</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_MIDIOUT</td>
<td>The <i>hmxobj</i> parameter is the identifier of a MIDI output device. This identifier must be in the range of zero to one less than the number of devices returned by the <a href="https://msdn.microsoft.com/f7abf545-3072-478e-9f6e-28b5fb6ab6e5">midiOutGetNumDevs</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_MIXER</td>
<td>The <i>hmxobj</i> parameter is the identifier of a mixer device in the range of zero to one less than the number of devices returned by the <a href="https://msdn.microsoft.com/ae3c3a28-1dc1-4e35-99d6-68e629124a89">mixerGetNumDevs</a> function. This flag is optional.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_WAVEIN</td>
<td>The <i>hmxobj</i> parameter is the identifier of a waveform-audio input device in the range of zero to one less than the number of devices returned by the <a href="https://msdn.microsoft.com/d8cb3c6c-edf7-4035-86da-b13fbdeddf6d">waveInGetNumDevs</a> function.</td>
</tr>
<tr>
<td>MIXER_OBJECTF_WAVEOUT</td>
<td>The <i>hmxobj</i> parameter is the identifier of a waveform-audio output device in the range of zero to one less than the number of devices returned by the <a href="https://msdn.microsoft.com/d9669c1c-36e2-4575-bf88-41c344d9c593">waveOutGetNumDevs</a> function.</td>
</tr>
</table>
 


## -returns



Returns MMSYSERR_NOERROR if successful or an error otherwise. Possible error values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MIXERR_INVALCONTROL</b></dt>
</dl>
</td>
<td width="60%">
The control reference is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MIXERR_INVALLINE</b></dt>
</dl>
</td>
<td width="60%">
The audio line reference is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_BADDEVICEID</b></dt>
</dl>
</td>
<td width="60%">
The <i>hmxobj</i> parameter specifies an invalid device identifier.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_INVALFLAG</b></dt>
</dl>
</td>
<td width="60%">
One or more flags are invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_INVALHANDLE</b></dt>
</dl>
</td>
<td width="60%">
The <i>hmxobj</i> parameter specifies an invalid handle.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_INVALPARAM</b></dt>
</dl>
</td>
<td width="60%">
One or more parameters are invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NODRIVER</b></dt>
</dl>
</td>
<td width="60%">
No mixer device is available for the object specified by <i>hmxobj</i>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/19f53a98-1a01-4954-a5d7-c428aa2bfa38">Audio Mixer Functions</a>



<a href="https://msdn.microsoft.com/7489fcac-fd4c-46cf-8a1a-e4de576974f0">Audio Mixers</a>
 

 

