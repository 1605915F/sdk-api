---
UID: NF:directmanipulation.IDirectManipulationViewport.GetStatus
title: IDirectManipulationViewport::GetStatus
author: windows-sdk-content
description: Gets the state of the viewport.
old-location: directmanipulation\idirectmanipulationviewport_getstatus.htm
tech.root: directmanipulation
ms.assetid: 1c02b2b2-8291-4151-b9c9-d80bf71f5ef5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetStatus, GetStatus method [Direct Manipulation], GetStatus method [Direct Manipulation],IDirectManipulationViewport interface, IDirectManipulationViewport interface [Direct Manipulation],GetStatus method, IDirectManipulationViewport.GetStatus, IDirectManipulationViewport::GetStatus, directmanipulation.idirectmanipulationviewport_getstatus, directmanipulation/IDirectManipulationViewport::GetStatus
ms.topic: method
req.header: directmanipulation.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: DirectManipulation.idl
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
 - COM
api_location:
 - DirectManipulation.h
api_name:
 - IDirectManipulationViewport.GetStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirectManipulationViewport::GetStatus


## -description


Gets the state of the viewport.


## -parameters




### -param status [out, retval]

One of the values from <a href="https://msdn.microsoft.com/6120702f-56f0-489d-a3b2-5f6ecac82b5e">DIRECTMANIPULATION_STATUS</a>.


## -returns



If the method succeeds, it returns <b>S_OK</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -remarks



This method returns the viewport state at the time of the call and not at the time when the return value is read.

This method will fail if called after <a href="https://msdn.microsoft.com/83d0bcde-03d2-4eba-991a-399b5307c8bd">Abandon</a>.


#### Examples

The following example shows how to use this method.

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>DIRECTMANIPULATION_STATUS status;

HRESULT hr = pViewport-&gt;GetStatus(&amp;status);
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/4c14143b-3b5f-401d-9df7-f17374abcd99">IDirectManipulationViewport</a>
 

 

