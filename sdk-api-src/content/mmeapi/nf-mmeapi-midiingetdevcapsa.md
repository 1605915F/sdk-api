---
UID: NF:mmeapi.midiInGetDevCapsA
title: midiInGetDevCapsA function
author: windows-sdk-content
description: The midiInGetDevCaps function determines the capabilities of a specified MIDI input device.
old-location: multimedia\midiingetdevcaps.htm
tech.root: Multimedia
ms.assetid: c3104427-69a9-434f-9f4e-780c96940c21
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_win32_midiInGetDevCaps, midiInGetDevCaps, midiInGetDevCaps function [Windows Multimedia], midiInGetDevCapsA, midiInGetDevCapsW, mmeapi/midiInGetDevCaps, mmeapi/midiInGetDevCapsA, mmeapi/midiInGetDevCapsW, multimedia.midiingetdevcaps"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: mmeapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: midiInGetDevCapsW (Unicode) and midiInGetDevCapsA (ANSI)
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
 - midiInGetDevCaps
 - midiInGetDevCapsA
 - midiInGetDevCapsW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# midiInGetDevCapsA function


## -description



The <b>midiInGetDevCaps</b> function determines the capabilities of a specified MIDI input device.




## -parameters




### -param uDeviceID

Identifier of the MIDI input device. The device identifier varies from zero to one less than the number of devices present. This parameter can also be a properly cast device handle.


### -param pmic

Pointer to a <a href="https://msdn.microsoft.com/358f0d4e-afdd-4a20-9572-ebb6e0000780">MIDIINCAPS</a> structure that is filled with information about the capabilities of the device.


### -param cbmic

Size, in bytes, of the <a href="https://msdn.microsoft.com/358f0d4e-afdd-4a20-9572-ebb6e0000780">MIDIINCAPS</a> structure. Only <i>cbMidiInCaps</i> bytes (or less) of information is copied to the location pointed to by <i>lpMidiInCaps</i>. If <i>cbMidiInCaps</i> is zero, nothing is copied, and the function returns MMSYSERR_NOERROR.


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
<dt><b>MMSYSERR_BADDEVICEID</b></dt>
</dl>
</td>
<td width="60%">
The specified device identifier is out of range.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_INVALPARAM</b></dt>
</dl>
</td>
<td width="60%">
The specified pointer or structure is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NODRIVER</b></dt>
</dl>
</td>
<td width="60%">
The driver is not installed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NOMEM</b></dt>
</dl>
</td>
<td width="60%">
The system is unable to allocate or lock memory.

</td>
</tr>
</table>
 




## -remarks



To determine the number of MIDI input devices present on the system, use the <a href="https://msdn.microsoft.com/23303bb2-e053-4a19-a63a-4e017b861af6">midiInGetNumDevs</a> function.




## -see-also




<a href="https://msdn.microsoft.com/9aa9fd79-cd9e-4443-8715-142ea72b82c0">MIDI Functions</a>
 

 

