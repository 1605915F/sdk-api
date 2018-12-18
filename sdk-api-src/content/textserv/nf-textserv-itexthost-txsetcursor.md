---
UID: NF:textserv.ITextHost.TxSetCursor
title: ITextHost::TxSetCursor
author: windows-sdk-content
description: Establishes a new cursor shape (I-beam) in the text host's window.
old-location: controls\ITextHost_TxSetCursor.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\windowlessricheditcontrols\windowlessricheditcontrolsreference\windowlessricheditcontrolinterfaces\txsetcursor.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextHost interface [Windows Controls],TxSetCursor method, ITextHost.TxSetCursor, ITextHost::TxSetCursor, TxSetCursor, TxSetCursor method [Windows Controls], TxSetCursor method [Windows Controls],ITextHost interface, _win32_ITextHost_TxSetCursor, _win32_ITextHost_TxSetCursor_cpp, controls.ITextHost_TxSetCursor, controls._win32_ITextHost_TxSetCursor, textserv/ITextHost::TxSetCursor
ms.topic: method
req.header: textserv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.lib: 
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextHost.TxSetCursor
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextHost::TxSetCursor


## -description


Establishes a new cursor shape (I-beam) in the text host's window.


## -parameters




### -param hcur [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HCURSOR</a></b>

Handle to the cursor. 


### -param fText [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

If <b>TRUE</b>, indicates the caller is trying to set the text cursor. See the Remarks section for more information. 


## -returns



This method does not return a value.




## -remarks



This method may be called at any time, whether the control is active or inactive.

<b>TxSetCursor</b> should be called by the text services object to set the mouse cursor. If the <i>fText</i> parameter is <b>TRUE</b>, the text services object is trying to set the text cursor (the cursor appears as an I-beam when it is over text that is not selected). In this case, the host can set it to whatever the control MousePointer property is. This is required for Microsoft Visual Basic compatibility since, through the MousePointer property, the Visual Basic programmer has control over the shape of the mouse cursor.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb787615(v=VS.85).aspx">ITextHost</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787609(v=VS.85).aspx">Windowless Rich Edit Controls Overview</a>
 

 

