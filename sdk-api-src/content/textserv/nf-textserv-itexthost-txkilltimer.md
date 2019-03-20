---
UID: NF:textserv.ITextHost.TxKillTimer
title: ITextHost::TxKillTimer (textserv.h)
author: windows-sdk-content
description: Requests the text host to destroy the specified timer.
old-location: controls\ITextHost_TxKillTimer.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\windowlessricheditcontrols\windowlessricheditcontrolsreference\windowlessricheditcontrolinterfaces\itexthost\itexthosttxkilltimer.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextHost interface [Windows Controls],TxKillTimer method, ITextHost.TxKillTimer, ITextHost::TxKillTimer, TxKillTimer, TxKillTimer method [Windows Controls], TxKillTimer method [Windows Controls],ITextHost interface, _win32_ITextHost_TxKillTimer, _win32_ITextHost_TxKillTimer_cpp, controls.ITextHost_TxKillTimer, controls._win32_ITextHost_TxKillTimer, textserv/ITextHost::TxKillTimer
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
 - ITextHost.TxKillTimer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextHost::TxKillTimer


## -description


Requests the text host to destroy the specified timer.


## -parameters




### -param idTimer [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Identifier of the timer created by the <a href="https://msdn.microsoft.com/en-us/library/Bb787686(v=VS.85).aspx">ITextHost::TxSetTimer</a> method. 


## -returns



This method has no return value. 




## -remarks



This method may be called at any time, whether the control is active or inactive.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787615(v=VS.85).aspx">ITextHost</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787686(v=VS.85).aspx">TxSetTimer</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787609(v=VS.85).aspx">Windowless Rich Edit Controls</a>
 

 

