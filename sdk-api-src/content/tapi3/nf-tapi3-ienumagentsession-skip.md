---
UID: NF:tapi3.IEnumAgentSession.Skip
title: IEnumAgentSession::Skip (tapi3.h)
author: windows-sdk-content
description: The Skip method skips over the next specified number of elements in the enumeration sequence.
old-location: tapi3\ienumagentsession_skip.htm
tech.root: Tapi
ms.assetid: 57358984-b874-46ac-9370-aab6a5136b87
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumAgentSession interface [TAPI 2.2],Skip method, IEnumAgentSession.Skip, IEnumAgentSession::Skip, Skip, Skip method [TAPI 2.2], Skip method [TAPI 2.2],IEnumAgentSession interface, _tapi3_ienumagentsession_skip, tapi3.ienumagentsession_skip, tapi3cc/IEnumAgentSession::Skip
ms.topic: method
req.header: tapi3.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - IEnumAgentSession.Skip
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumAgentSession::Skip


## -description


The 
<b>Skip</b> method skips over the next specified number of elements in the enumeration sequence.


## -parameters




### -param celt [in]

Number of elements to skip.


## -returns



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
Number of elements skipped was <i>celt</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
Number of elements skipped was not <i>celt</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/38b9fc57-a0af-4dfa-9058-e721138c8be9">IEnumAgentSession</a>
 

 

