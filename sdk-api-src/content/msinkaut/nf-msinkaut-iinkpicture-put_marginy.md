---
UID: NF:msinkaut.IInkPicture.put_MarginY
title: IInkPicture::put_MarginY (msinkaut.h)
author: windows-sdk-content
description: Gets or sets the y-axis margin around the window rectangle, in screen coordinates.This margin provides a buffer around the edge of the ink window.
old-location: tablet\inkpicture_marginy.htm
tech.root: tablet
ms.assetid: f5320061-36c7-4dcb-b5d3-3df41ddcac2a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IInkPicture interface [Tablet PC],MarginY property, IInkPicture.MarginY, IInkPicture.put_MarginY, IInkPicture::MarginY, IInkPicture::get_MarginY, IInkPicture::put_MarginY, InkPicture.get_MarginY, InkPicture.put_MarginY, MarginY property [Tablet PC], MarginY property [Tablet PC],IInkPicture interface, get_MarginY, msinkaut/IInkPicture::MarginY, msinkaut/IInkPicture::get_MarginY, msinkaut/IInkPicture::put_MarginY, put_MarginY, tablet.inkpicture_marginy
ms.topic: method
req.header: msinkaut.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: InkObj.dll
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - InkObj.dll
 - InkObj.dll.dll
api_name:
 - IInkPicture.MarginY
 - IInkPicture.get_MarginY
 - IInkPicture.put_MarginY
 - InkPicture.get_MarginY
 - InkPicture.put_MarginY
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IInkPicture::put_MarginY


## -description



Gets or sets the y-axis margin around the window rectangle, in screen coordinates.

This margin provides a buffer around the edge of the ink window.



This property is read/write.


## -parameters


## -remarks



This property is most commonly used with nonintegrated tablet devices-the buffer gives users a margin of error when writing on a device that may not map 1 to 1 with the screen.

The margin is specified in screen coordinates. A positive margin extends outside the context, a negative margin extends inside the context, and a value of zero produces no margin. Ink is collected if the stroke starts within the margin. This behavior does not clip the ink. The context of the object or control is either the window input rectangle from the <a href="https://msdn.microsoft.com/975e5921-cc76-4b38-9f3c-364e8704ba03">GetWindowInputRectangle</a> method or the client rectangle for the window.

The margin is effective only within the application's window. If the pen is applied outside the application's window, then the application loses focus and cannot collect ink.

<div class="alert"><b>Note</b>  The <a href="https://msdn.microsoft.com/189f430e-9d00-4e29-bb8c-8ac195896793">InkCollector</a> object, the <a href="https://msdn.microsoft.com/61191ab3-075e-458b-9e0f-4bc255687b3c">InkOverlay</a> object, or the <a href="https://msdn.microsoft.com/e9fa6807-6e2a-44ec-9b8f-a560185e4367">InkPicture</a> control must be disabled before setting this property. To disable the <b>InkCollector</b> or <b>InkOverlay</b> object, set the <a href="https://msdn.microsoft.com/1c6e9fb4-be51-4d68-8241-17119deeba3f">Enabled</a> property to <b>FALSE</b>. To disable inking in the <b>InkOverlay</b> control, set the <a href="https://msdn.microsoft.com/3af59de9-0239-47ab-b3b3-1f1baecb169f">InkEnabled</a> property to <b>FALSE</b>. You can then set the <b>MarginY</b> property, and re-enable the object or control by setting the <b>Enabled</b> property (or <b>InkEnabled</b> property) to <b>TRUE</b>.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/1c6e9fb4-be51-4d68-8241-17119deeba3f">Enabled Property</a>



<a href="https://msdn.microsoft.com/en-us/library/Mt846800(v=VS.85).aspx">IInkPicture</a>



<a href="https://msdn.microsoft.com/3af59de9-0239-47ab-b3b3-1f1baecb169f">InkEnabled Property</a>



<a href="https://msdn.microsoft.com/1ced9779-dae5-4f9a-8a68-b2c0d041d5b4">InkPicture Control</a>



<a href="https://msdn.microsoft.com/c463debc-341b-4491-8543-70623bf717d0">MarginX Property</a>
 

 

