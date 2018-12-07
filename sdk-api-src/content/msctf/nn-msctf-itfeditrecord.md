---
UID: NN:msctf.ITfEditRecord
title: ITfEditRecord
author: windows-sdk-content
description: The ITfEditRecord interface is implemented by the TSF manager and is used by a text edit sink to determine what was changed during an edit session.
old-location: tsf\itfeditrecord.htm
tech.root: TSF
ms.assetid: 2106cd97-9e1f-4d7c-a7a4-55676cf8923b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITfEditRecord, ITfEditRecord interface [Text Services Framework], ITfEditRecord interface [Text Services Framework],described, _tsf_itfeditrecord_ref, msctf/ITfEditRecord, tsf.itfeditrecord
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: msctf.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
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
 - msctf.dll
api_name:
 - ITfEditRecord
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfEditRecord interface


## -description


The <b>ITfEditRecord</b> interface is implemented by the TSF manager and is used by a text edit sink to determine what was changed during an edit session. An instance of this interface is passed to the text edit sink when the <a href="https://msdn.microsoft.com/7763a879-a558-463d-837b-e38e6f84b9f7">ITfTextEditSink::OnEndEdit</a> method is called.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ITfEditRecord</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>ITfEditRecord</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ITfEditRecord</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ad7dbd71-6241-45a0-9815-1f0eedc5213a">GetSelectionStatus</a>
</td>
<td align="left" width="63%">
Determines if the selection has changed during the edit session.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/bfc9cba0-298c-4823-b70a-366bdc5bfb29">GetTextAndPropertyUpdates</a>
</td>
<td align="left" width="63%">
Obtains an enumerator that contains a collection of range objects that cover the specified properties and/or text that changed during the edit session.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/7763a879-a558-463d-837b-e38e6f84b9f7">ITfTextEditSink::OnEndEdit
      </a>



<a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a>
 

 

