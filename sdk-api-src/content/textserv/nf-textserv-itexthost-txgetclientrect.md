---
UID: NF:textserv.ITextHost.TxGetClientRect
title: ITextHost::TxGetClientRect
author: windows-sdk-content
description: Retrieves the client coordinates of the text host's client area.
old-location: controls\ITextHost_TxGetClientRect.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\windowlessricheditcontrols\windowlessricheditcontrolsreference\windowlessricheditcontrolinterfaces\txgetclientrect.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextHost interface [Windows Controls],TxGetClientRect method, ITextHost.TxGetClientRect, ITextHost::TxGetClientRect, TxGetClientRect, TxGetClientRect method [Windows Controls], TxGetClientRect method [Windows Controls],ITextHost interface, _win32_ITextHost_TxGetClientRect, _win32_ITextHost_TxGetClientRect_cpp, controls.ITextHost_TxGetClientRect, controls._win32_ITextHost_TxGetClientRect, textserv/ITextHost::TxGetClientRect
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
 - ITextHost.TxGetClientRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextHost::TxGetClientRect


## -description


Retrieves the client coordinates of the text host's client area.


## -parameters




### -param prc

Type: <b>LPRECT</b>

The client coordinates of the text host's client area. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Return S_OK if the method succeeds. 

Return the following COM error code if the method fails. For more information on COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
Unspecified error.

</td>
</tr>
</table>
 




## -remarks



The client rectangle is the rectangle that the text services object is responsible for painting and managing. The host relies on the text services object for painting that area. And, the text services object must not paint or invalidate areas outside of that rectangle.

The host forwards mouse messages to the text services object when the cursor is over the client rectangle.

The client rectangle is expressed in client coordinates of the containing window.

<div class="alert"><b>Important</b>  The <b>ITextHost::TxGetClientRect</b> method will fail if called at an inactive time.</div>
<div> </div>



## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787615(v=VS.85).aspx">ITextHost</a>



<b>Other Resources</b>



<a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787609(v=VS.85).aspx">Windowless Rich Edit Controls</a>
 

 

