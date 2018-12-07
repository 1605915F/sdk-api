---
UID: NF:textserv.ITextHost.TxActivate
title: ITextHost::TxActivate
author: windows-sdk-content
description: Notifies the text host that the control is active.
old-location: controls\ITextHost_TxActivate.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\windowlessricheditcontrols\windowlessricheditcontrolsreference\windowlessricheditcontrolinterfaces\txactivate.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextHost interface [Windows Controls],TxActivate method, ITextHost.TxActivate, ITextHost::TxActivate, TxActivate, TxActivate method [Windows Controls], TxActivate method [Windows Controls],ITextHost interface, _win32_ITextHost_TxActivate, _win32_ITextHost_TxActivate_cpp, controls.ITextHost_TxActivate, controls._win32_ITextHost_TxActivate, textserv/ITextHost::TxActivate
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ITextHost.TxActivate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextHost::TxActivate


## -description


Notifies the text host that the control is active.


## -parameters




### -param plOldState

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a>*</b>

The previous activation state. 


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
Activation is not possible at this time.

</td>
</tr>
</table>
 




## -remarks



It is legal for the host to refuse an activation request; for example, the control may be minimized and thus invisible.

The caller should be able to gracefully handle failure to activate.

No matter how many times this method is called, only one <a href="https://msdn.microsoft.com/en-us/library/Bb787642(v=VS.85).aspx">ITextHost::TxDeactivate</a> call is necessary to deactivate the control.

This function returns an opaque handle in 
				<i>plOldState</i>. The caller (the text services object) should save this handle and use it in a subsequent call to <a href="https://msdn.microsoft.com/en-us/library/Bb787642(v=VS.85).aspx">ITextHost::TxDeactivate</a>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787615(v=VS.85).aspx">ITextHost</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787642(v=VS.85).aspx">TxDeactivate</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787609(v=VS.85).aspx">Windowless Rich Edit Controls</a>
 

 

