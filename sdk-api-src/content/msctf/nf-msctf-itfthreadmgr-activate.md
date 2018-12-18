---
UID: NF:msctf.ITfThreadMgr.Activate
title: ITfThreadMgr::Activate
author: windows-sdk-content
description: ITfThreadMgr::Activate method
old-location: tsf\itfthreadmgr_activate.htm
tech.root: TSF
ms.assetid: bd9058c0-55b0-4231-a336-7cea4db75c0f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Activate, Activate method [Text Services Framework], Activate method [Text Services Framework],ITfThreadMgr interface, ITfThreadMgr interface [Text Services Framework],Activate method, ITfThreadMgr.Activate, ITfThreadMgr::Activate, _tsf_itfthreadmgr_activate_ref, msctf/ITfThreadMgr::Activate, tsf.itfthreadmgr_activate
ms.topic: method
req.header: msctf.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Msctf.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Msctf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msctf.dll
api_name:
 - ITfThreadMgr.Activate
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfThreadMgr::Activate


## -description




## -parameters




### -param ptid [out]

Pointer to a <a href="https://msdn.microsoft.com/984dc390-6e15-4491-8c06-77c27c5bdd6f">TfClientId</a> value that receives a client identifier.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
<i>ptid</i> is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
This method was called while the thread was deactivating.

</td>
</tr>
</table>
 




## -remarks



This method can be called more than once from a thread, but each call must be matched with a corresponding call to <a href="https://msdn.microsoft.com/7293fbfa-c385-4713-80b2-760e54dbf4c1">ITfThreadMgr::Deactivate</a> from the same thread.




## -see-also




<a href="https://msdn.microsoft.com/3a2ba59c-3565-4f54-ac10-923dcb4882cb">ITfThreadMgr</a>



<a href="https://msdn.microsoft.com/7293fbfa-c385-4713-80b2-760e54dbf4c1">ITfThreadMgr::Deactivate
      </a>



<a href="https://msdn.microsoft.com/984dc390-6e15-4491-8c06-77c27c5bdd6f">TfClientId
      </a>
 

 

