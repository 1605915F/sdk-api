---
UID: NF:amvideo.IFullScreenVideoEx.IsModeAvailable
title: IFullScreenVideoEx::IsModeAvailable
author: windows-sdk-content
description: The IsModeAvailable method queries whether a specified display mode is available.
old-location: dshow\ifullscreenvideoex_ismodeavailable.htm
tech.root: DirectShow
ms.assetid: 9b05d6c6-522c-46b8-90b5-c4650cee5f6b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFullScreenVideoEx interface [DirectShow],IsModeAvailable method, IFullScreenVideoEx.IsModeAvailable, IFullScreenVideoEx::IsModeAvailable, IFullScreenVideoIsModeAvailable, IsModeAvailable, IsModeAvailable method [DirectShow], IsModeAvailable method [DirectShow],IFullScreenVideoEx interface, amvideo/IFullScreenVideoEx::IsModeAvailable, dshow.ifullscreenvideoex_ismodeavailable
ms.topic: method
req.header: amvideo.h
req.include-header: Dshow.h
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IFullScreenVideoEx.IsModeAvailable
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFullScreenVideoEx::IsModeAvailable


## -description



The <code>IsModeAvailable</code> method queries whether a specified display mode is available.




## -parameters




### -param Mode [in]

Index of the display mode.


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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Index out of range.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The display mode is not available.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The display mode is available.

</td>
</tr>
</table>
 




## -remarks



The Full Screen Renderer supports a static set of display modes. However, the video card on the user's system might not support every mode. If a particular display mode is not supported by the video card, this method returns S_FALSE. Even if a particular mode is available, it will not necessarily be used for video playback. The mode must also be compatible with the filters in the filter graph.

You can disable a display mode by calling the <a href="https://msdn.microsoft.com/en-us/library/Dd390075(v=VS.85).aspx">IFullScreenVideoEx::SetEnabled</a> method. The Full Screen Renderer will not use a disabled mode, even if the video card supports it.

Display modes are indexed from zero. The <a href="https://msdn.microsoft.com/en-us/library/Dd390057(v=VS.85).aspx">IFullScreenVideoEx::CountModes</a> method returns the number of modes.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd390056(v=VS.85).aspx">IFullScreenVideoEx Interface</a>
 

 

