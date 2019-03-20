---
UID: NN:imapi.IRedbookDiscMaster
title: IRedbookDiscMaster (imapi.h)
author: windows-sdk-content
description: The IRedbookDiscMaster interface enables the staging of an audio CD image. It represents one of the formats supported by MSDiscMasterObj, and it allows the creation of multi-track audio discs in Track-at-Once mode (fixed-size audio gaps).
old-location: imapi\iredbookdiscmaster.htm
tech.root: imapi
ms.assetid: ea531b22-869a-400e-801f-00bb85ebaac2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IRedbookDiscMaster, IRedbookDiscMaster interface [IMAPI], IRedbookDiscMaster interface [IMAPI],described, _win32_iredbookdiscmaster, base.iredbookdiscmaster, imapi.iredbookdiscmaster, imapi/IRedbookDiscMaster
ms.topic: interface
req.header: imapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Actxprxy.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Actxprxy.dll
api_name:
 - IRedbookDiscMaster
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRedbookDiscMaster interface


## -description


The 
<b>IRedbookDiscMaster</b> interface enables the staging of an audio CD image. It represents one of the formats supported by <b>MSDiscMasterObj</b>, and it allows the creation of multi-track audio discs in Track-at-Once mode (fixed-size audio gaps).

Tracks are created in the stash file, data is added to them, and then they are closed. Only one track is staged at a time; this is called the <i>open track</i>. The remaining tracks are closed and committed to the image, while the open track has available to it all the blocks that are not in use by closed tracks.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IRedbookDiscMaster</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IRedbookDiscMaster</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IRedbookDiscMaster</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d9bd4f3c-4ff5-4f6e-9520-27fef3736636">AddAudioTrackBlocks</a>
</td>
<td align="left" width="63%">
Adds blocks of audio to a track being staged.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/01ec0eba-d592-46eb-8029-86cb678b8b34">CloseAudioTrack</a>
</td>
<td align="left" width="63%">
Closes out staging of an audio track.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b0300cd8-08e9-434e-9c1b-c33a19148e7e">CreateAudioTrack</a>
</td>
<td align="left" width="63%">
Begins staging a new audio track.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/25e8fd75-7a24-421f-b61e-b131dfbbcc8c">GetAudioBlockSize</a>
</td>
<td align="left" width="63%">
Retrieves the audio block size in bytes (2352).

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/57647490-0384-4cdb-842f-f1fb16dd2096">GetAvailableAudioTrackBlocks</a>
</td>
<td align="left" width="63%">
Retrieves the blocks available for current track.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c4b0f02e-d881-4a4f-9356-d8232ef4c297">GetTotalAudioBlocks</a>
</td>
<td align="left" width="63%">
Retrieves the total audio blocks available on disc.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ef284941-0724-4e0a-8ce9-c47d5a53a30e">GetTotalAudioTracks</a>
</td>
<td align="left" width="63%">
Retrieves the total tracks staged in the image.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/32921d7f-9cb2-4ae4-9064-18df91a237ba">GetUsedAudioBlocks</a>
</td>
<td align="left" width="63%">
Retrieves total audio blocks staged in image.

</td>
</tr>
</table> 

