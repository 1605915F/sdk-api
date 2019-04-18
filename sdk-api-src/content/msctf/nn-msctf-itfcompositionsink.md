---
UID: NN:msctf.ITfCompositionSink
title: ITfCompositionSink (msctf.h)
author: windows-sdk-content
description: The ITfCompositionSink interface is implemented by a text service to receive a notification when a composition is terminated.
old-location: tsf\itfcompositionsink.htm
tech.root: TSF
ms.assetid: 17d5eab5-a308-40a5-823a-f176508dda71
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITfCompositionSink, ITfCompositionSink interface [Text Services Framework], ITfCompositionSink interface [Text Services Framework],described, _tsf_itfcompositionsink_ref, msctf/ITfCompositionSink, tsf.itfcompositionsink
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
req.dll: Imekrcic.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - imekrcic.dll
api_name:
 - ITfCompositionSink
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
ms.custom: 19H1
---

# ITfCompositionSink interface


## -description


The <b>ITfCompositionSink</b> interface is implemented by a text service to receive a notification when a composition is terminated. This advise sink is installed by passing a pointer to this interface when the composition is started with the <a href="https://msdn.microsoft.com/aab84e6c-39c7-438e-b4f0-1d174473aa02">ITfContextComposition::StartComposition</a> method.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ITfCompositionSink</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>ITfCompositionSink</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ITfCompositionSink</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4b7c3993-6d01-492f-9bb5-241a1cbd4b63">OnCompositionTerminated</a>
</td>
<td align="left" width="63%">
Called when a composition is terminated.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/aab84e6c-39c7-438e-b4f0-1d174473aa02">ITfContextComposition::StartComposition
      </a>



<a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a>
 

 

