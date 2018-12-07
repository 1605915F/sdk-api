---
UID: NF:mmeapi.waveInGetPosition
title: waveInGetPosition function
author: windows-sdk-content
description: waveInGetPosition is no longer supported for use as of Windows Vista.
old-location: multimedia\waveingetposition.htm
tech.root: Multimedia
ms.assetid: 91764c6e-e9d4-4d8e-819a-6e27ca2478d8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_win32_waveInGetPosition, mmeapi/waveInGetPosition, multimedia.waveingetposition, waveInGetPosition, waveInGetPosition function [Windows Multimedia]"
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
req.unicode-ansi: 
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
 - waveInGetPosition
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# waveInGetPosition function


## -description


<p class="CCE_Message">[<b>waveInGetPosition</b> is no longer supported for use as of Windows Vista. Instead, use <a href="https://msdn.microsoft.com/2271bd73-8cb6-4048-a16c-f765d0fae6bd">IAudioClock::GetPosition</a>.]

The <b>waveInGetPosition</b> function retrieves the current input position of the given waveform-audio input device.


## -parameters




### -param hwi

Handle to the waveform-audio input device.
          


### -param pmmt

Pointer to an <a href="https://msdn.microsoft.com/94bb7235-2477-4923-add8-f0c8ac8195c2">MMTIME</a> structure.
          


### -param cbmmt

Size, in bytes, of the <a href="https://msdn.microsoft.com/94bb7235-2477-4923-add8-f0c8ac8195c2">MMTIME</a> structure.
          


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
<dt><b>MMSYSERR_INVALHANDLE</b></dt>
</dl>
</td>
<td width="60%">
Specified device handle is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NODRIVER</b></dt>
</dl>
</td>
<td width="60%">
No device driver is present.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NOMEM</b></dt>
</dl>
</td>
<td width="60%">
Unable to allocate or lock memory.

</td>
</tr>
</table>
 




## -remarks



Before calling this function, set the <b>wType</b> member of the <a href="https://msdn.microsoft.com/94bb7235-2477-4923-add8-f0c8ac8195c2">MMTIME</a> structure to indicate the time format you want. After calling this function, check <b>wType</b> to determine whether the desired time format is supported. If the format is not supported, the member will specify an alternative format.

The position is set to zero when the device is opened or reset.




## -see-also




<a href="https://msdn.microsoft.com/3188355c-65be-4372-8e87-e7f755982592">Waveform Audio</a>



<a href="https://msdn.microsoft.com/6c8aaa54-0477-484f-91e1-d2152aa9c185">Waveform Functions</a>
 

 

