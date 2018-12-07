---
UID: NF:msctf.ITfMessagePump.PeekMessageA
title: ITfMessagePump::PeekMessageA
author: windows-sdk-content
description: ITfMessagePump::PeekMessageA method
old-location: tsf\itfmessagepump_peekmessagea.htm
tech.root: TSF
ms.assetid: 4b20fa18-f5c3-4f3b-bb93-0e352d620d31
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITfMessagePump interface [Text Services Framework],PeekMessageA method, ITfMessagePump.PeekMessageA, ITfMessagePump::PeekMessageA, PeekMessageA, PeekMessageA method [Text Services Framework], PeekMessageA method [Text Services Framework],ITfMessagePump interface, _tsf_itfmessagepump_peekmessagea_ref, msctf/ITfMessagePump::PeekMessageA, tsf.itfmessagepump_peekmessagea
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ITfMessagePump.PeekMessageA
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfMessagePump::PeekMessageA


## -description




## -parameters




### -param pMsg [out]

Pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms644958(v=VS.85).aspx">MSG</a> structure that receives message data.


### -param hwnd [in]

Handle to the window whose messages are obtained. The window must belong to the current thread. If this value is <b>NULL</b>, this method obtains messages for any window owned by the calling thread.


### -param wMsgFilterMin [in]

Specifies the lowest message value to obtain.


### -param wMsgFilterMax [in]

Specifies the highest message value to obtain.


### -param wRemoveMsg [in]

Specifies how messages are handled. For more information, see the <b>PeekMessage</b> function.


### -param pfResult [out]

Pointer to a BOOL that receives the return value from the <b>PeekMessage</b> function.


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
One or more parameters are invalid.

</td>
</tr>
</table>
 




## -remarks



If <i>wMsgFilterMin</i> and <i>wMsgFilterMax</i> are both zero, this method returns all available messages; that is, no range filtering is performed.




## -see-also




<a href="https://msdn.microsoft.com/f7c3d039-cffc-4ce0-8579-041ba849de6d">ITfMessagePump</a>



<a href="https://msdn.microsoft.com/en-us/library/ms644958(v=VS.85).aspx">MSG</a>



<a href="https://msdn.microsoft.com/en-us/library/ms644943(v=VS.85).aspx">PeekMessage</a>
 

 

