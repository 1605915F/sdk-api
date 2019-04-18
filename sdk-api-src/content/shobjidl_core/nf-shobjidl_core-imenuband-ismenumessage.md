---
UID: NF:shobjidl_core.IMenuBand.IsMenuMessage
title: IMenuBand::IsMenuMessage (shobjidl_core.h)
author: windows-sdk-content
description: A message pump calls this method to see if any messages should be redirected to the Component Object Model (COM) object.
old-location: shell\IMenuBand_IsMenuMessage.htm
tech.root: shell
ms.assetid: d30a456c-7c09-4250-8509-353c54d017b9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IMenuBand interface [Windows Shell],IsMenuMessage method, IMenuBand.IsMenuMessage, IMenuBand::IsMenuMessage, IsMenuMessage, IsMenuMessage method [Windows Shell], IsMenuMessage method [Windows Shell],IMenuBand interface, _shell_IMenuBand_IsMenuMessage, shell.IMenuBand_IsMenuMessage, shobjidl_core/IMenuBand::IsMenuMessage
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Shell32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Shell32.dll
api_name:
 - IMenuBand.IsMenuMessage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMenuBand::IsMenuMessage


## -description


A message pump calls this method to see if any messages should be redirected to the Component Object Model (COM) object.


## -parameters




### -param pmsg [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms644958(v=VS.85).aspx">MSG</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/en-us/library/ms644958(v=VS.85).aspx">MSG</a> structure.


## -returns



Type: <b>HRESULT</b>

This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
A message should be redirected to the COM object. The application should call <a href="https://msdn.microsoft.com/5ee1f64f-ca8b-4f50-bbab-24ff1216708c">IMenuBand::TranslateMenuMessage</a> with this message.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The menu has exited the menu mode and can be destroyed.

</td>
</tr>
</table>
 




## -remarks



If this method returns <b>S_OK</b>, the message loop should not call <a href="https://msdn.microsoft.com/en-us/library/ms644955(v=VS.85).aspx">TranslateMessage</a> or <a href="https://msdn.microsoft.com/en-us/library/ms644934(v=VS.85).aspx">DispatchMessage</a>.



