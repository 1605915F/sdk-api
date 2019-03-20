---
UID: NF:amvideo.IFullScreenVideoEx.SetCaption
title: IFullScreenVideoEx::SetCaption (amvideo.h)
author: windows-sdk-content
description: The SetCaption method sets the caption associated with the full-screen window.
old-location: dshow\ifullscreenvideoex_setcaption.htm
tech.root: DirectShow
ms.assetid: 6f520ab4-867f-4001-8f2f-25f0d8efe454
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFullScreenVideoEx interface [DirectShow],SetCaption method, IFullScreenVideoEx.SetCaption, IFullScreenVideoEx::SetCaption, IFullScreenVideoSetCaption, SetCaption, SetCaption method [DirectShow], SetCaption method [DirectShow],IFullScreenVideoEx interface, amvideo/IFullScreenVideoEx::SetCaption, dshow.ifullscreenvideoex_setcaption
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
 - IFullScreenVideoEx.SetCaption
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFullScreenVideoEx::SetCaption


## -description



The <code>SetCaption</code> method sets the caption associated with the full-screen window.




## -parameters




### -param strCaption [in]

String containing the caption.


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
<b>NULL</b> pointer argument.

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
 




## -remarks



The caption is visible when the window is minimized.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd390056(v=VS.85).aspx">IFullScreenVideoEx Interface</a>
 

 

