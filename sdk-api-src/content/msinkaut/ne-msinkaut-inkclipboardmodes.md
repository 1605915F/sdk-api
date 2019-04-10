---
UID: NE:msinkaut.InkClipboardModes
title: InkClipboardModes (msinkaut.h)
author: windows-sdk-content
description: Specifies the copy options of the Clipboard.
old-location: tablet\inkclipboardmodes.htm
tech.root: tablet
ms.assetid: a9718b79-8f98-4bfc-a5db-208899d1f59e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ICB_Copy, ICB_Cut, ICB_Default, ICB_DelayedCopy, ICB_ExtractOnly, InkClipboardModes, InkClipboardModes enumeration [Tablet PC], a9718b79-8f98-4bfc-a5db-208899d1f59e, msinkaut/ICB_Copy, msinkaut/ICB_Cut, msinkaut/ICB_Default, msinkaut/ICB_DelayedCopy, msinkaut/ICB_ExtractOnly, msinkaut/InkClipboardModes, tablet.inkclipboardmodes
ms.topic: enum
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - msinkaut.h
api_name:
 - InkClipboardModes
product: Windows
targetos: Windows
req.typenames: InkClipboardModes
req.redist: 
---

# InkClipboardModes enumeration


## -description



Specifies the copy options of the Clipboard.




## -enum-fields




### -field ICB_Copy

The ink is copied to the Clipboard.


### -field ICB_Cut

The ink is cut and copied to the Clipboard.


### -field ICB_ExtractOnly

The ink is not copied to the Clipboard. Typically, use this option if you want to add something else, such as text, to the ink before you copy it to the Clipboard.


### -field ICB_DelayedCopy

 Delayed rendering is used to reduce the amount of data that is stored on the Clipboard. The data is rendered when a paste request is made.


### -field ICB_Default

Copy mode is used to copy the Ink.


## -remarks



You can use the DelayedCopy flag to interact directly with the data object and add additional formats to the clipboard.

<div class="alert"><b>Caution</b>  To avoid potential memory leaks as a result of using the <b>DelayedCopy</b> flag, you must call the <a href="https://msdn.microsoft.com/en-us/library/ms679707(v=VS.85).aspx">OleFlushClipboard</a> or <a href="https://msdn.microsoft.com/en-us/library/ms686623(v=VS.85).aspx">OleSetClipboard</a> method. This must be done before the application exits if the last call to the <a href="https://msdn.microsoft.com/ad62c9b3-6df6-445b-9085-7cd5c4b6b31f">ClipboardCopy</a> method used the <b>DelayedCopy</b> flag.</div>
<div> </div>
To remove the pointer from the clipboard, the parameter for the <a href="https://msdn.microsoft.com/en-us/library/ms686623(v=VS.85).aspx">OleSetClipboard</a> should be <b>NULL</b>. For the <a href="https://msdn.microsoft.com/en-us/library/Hh706940(v=VS.85).aspx">SetDataObject</a> method, the <i>data</i> parameter should be <b>NULL</b>, and the <i>copy</i> parameter should be <b>TRUE</b>.

The <a href="https://msdn.microsoft.com/en-us/library/ms686623(v=VS.85).aspx">OleSetClipboard</a> and <a href="https://msdn.microsoft.com/en-us/library/Hh706940(v=VS.85).aspx">SetDataObject</a> methods replace the contents of the clipboard.




## -see-also




<a href="https://msdn.microsoft.com/ad62c9b3-6df6-445b-9085-7cd5c4b6b31f">ClipboardCopy Method</a>



<a href="https://msdn.microsoft.com/a4e6a183-242a-40af-871b-43a0b177a27a">ClipboardCopyWithRectangle Method</a>



<a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp Class</a>
 

 

