---
UID: NF:mfidl.IMFTranscodeProfile.GetAudioAttributes
title: IMFTranscodeProfile::GetAudioAttributes (mfidl.h)
author: windows-sdk-content
description: Gets the audio stream settings that are currently set in the transcode profile.
old-location: mf\imftranscodeprofile_getaudioattributes.htm
tech.root: medfound
ms.assetid: c02dabfe-33ef-4835-a707-d1350b18629f
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetAudioAttributes, GetAudioAttributes method [Media Foundation], GetAudioAttributes method [Media Foundation],IMFTranscodeProfile interface, IMFTranscodeProfile interface [Media Foundation],GetAudioAttributes method, IMFTranscodeProfile.GetAudioAttributes, IMFTranscodeProfile::GetAudioAttributes, mf.imftranscodeprofile_getaudioattributes, mfidl/IMFTranscodeProfile::GetAudioAttributes
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mfidl.idl
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
 - mfidl.h
api_name:
 - IMFTranscodeProfile.GetAudioAttributes
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFTranscodeProfile::GetAudioAttributes


## -description


Gets the audio stream settings that are currently set in the transcode profile.
  


## -parameters




### -param ppAttrs [out]

Receives a pointer to the <a href="https://msdn.microsoft.com/e12259f4-b631-4d4a-a296-c1cc6334b962">IMFAttributes</a> interface of the attribute store containing the current audio stream settings. Caller must release the interface pointer.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



If there are no audio attributes set in the transcode profile, the call to <b>GetAudioAttributes</b> succeeds and  <i>ppAttrs</i> receives <b>NULL</b>.

To get a specific attribute value, the caller must call the appropriate <a href="https://msdn.microsoft.com/e12259f4-b631-4d4a-a296-c1cc6334b962">IMFAttributes</a> method depending on the data type of the attribute, and specify the attribute name. The following topics describe the audio attributes:

<ul>
<li>
<a href="https://msdn.microsoft.com/15aad4ea-7b4b-4a6f-bac7-18e0c281f2a6">Audio Media Types</a>
</li>
<li>
<a href="https://msdn.microsoft.com/9a6b6402-ff53-4399-8616-06b7768a8737">MF_TRANSCODE_ENCODINGPROFILE</a>
</li>
<li>
<a href="https://msdn.microsoft.com/872140e8-fd39-446c-a84f-1e04ea95076e">MF_TRANSCODE_QUALITYVSSPEED</a>
</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/44af5e03-5f0a-4564-b9d6-b8c935df35b2">Attributes in Media Foundation</a>



<a href="https://msdn.microsoft.com/82e012e0-84d8-4791-8b6f-bda58b498a90">IMFTranscodeProfile</a>



<a href="https://msdn.microsoft.com/24bf68a8-39bf-4302-b28c-71bb23b63469">Transcode API</a>
 

 

