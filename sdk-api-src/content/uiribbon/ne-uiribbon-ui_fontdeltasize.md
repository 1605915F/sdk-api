---
UID: NE:uiribbon.UI_FONTDELTASIZE
title: UI_FONTDELTASIZE
author: windows-sdk-content
description: Specifies values that identify whether the font size of a highlighted text run should be incremented or decremented.
old-location: windowsribbon\windowsribbon_ui_fontdeltasize.htm
tech.root: windowsribbon
ms.assetid: VS|scenicintent|~\scenicintent\reference\enums\ui_fontdeltasize.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: UI_FONTDELTASIZE, UI_FONTDELTASIZE enumeration [Windows Ribbon], UI_FONTDELTASIZE_GROW, UI_FONTDELTASIZE_SHRINK, scenicintent_UI_FONTDELTASIZE, uiribbon/UI_FONTDELTASIZE, uiribbon/UI_FONTDELTASIZE_GROW, uiribbon/UI_FONTDELTASIZE_SHRINK, windowsribbon.windowsribbon_ui_fontdeltasize
ms.topic: enum
req.header: uiribbon.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Uiribbon.idl
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
 - Uiribbon.h
api_name:
 - UI_FONTDELTASIZE
product: Windows
targetos: Windows
req.typenames: UI_FONTDELTASIZE
req.redist: 
---

# UI_FONTDELTASIZE enumeration


## -description


Specifies values that identify whether the font size of a highlighted text run should be incremented or decremented.


## -enum-fields




### -field UI_FONTDELTASIZE_GROW

Increment the font size.


### -field UI_FONTDELTASIZE_SHRINK

Decrement the font size.


## -remarks



When you highlight a run of heterogeneously sized text, the Ribbon framework sets the <b>Font size</b> control to blank.  When you click the <b>Font grow</b> button or the <b>Font shrink</b> button, the highlighted text is resized, and the relative size variations in the text run are maintained.

The following screen shot shows the <b>Font grow</b> and <b>Font shrink</b> buttons on the <a href="https://msdn.microsoft.com/en-us/library/Dd371673(v=VS.85).aspx">FontControl</a>.

<img alt="Screen shot of the Font grow and Font shrink buttons on the FontControl." src="./images/FontControl_IncDec.png"/>




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd371540(v=VS.85).aspx">Constants and Enumerations</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd371211(v=VS.85).aspx">UI_PKEY_FontProperties_DeltaSize</a>
 

 

