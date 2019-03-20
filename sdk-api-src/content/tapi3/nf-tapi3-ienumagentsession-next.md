---
UID: NF:tapi3.IEnumAgentSession.Next
title: IEnumAgentSession::Next (tapi3.h)
author: windows-sdk-content
description: The Next method gets the next specified number of elements in the enumeration sequence.
old-location: tapi3\ienumagentsession_next.htm
tech.root: Tapi
ms.assetid: 5ac647a0-7f1a-4f6a-ad01-dba019f9bf56
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumAgentSession interface [TAPI 2.2],Next method, IEnumAgentSession.Next, IEnumAgentSession::Next, Next, Next method [TAPI 2.2], Next method [TAPI 2.2],IEnumAgentSession interface, _tapi3_ienumagentsession_next, tapi3.ienumagentsession_next, tapi3cc/IEnumAgentSession::Next
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
 - IEnumAgentSession.Next
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumAgentSession::Next


## -description


The 
<b>Next</b> method gets the next specified number of elements in the enumeration sequence.


## -parameters




### -param celt [in]

Number of elements requested.


### -param ppElements [out]

Pointer to 
<a href="https://msdn.microsoft.com/b0db0834-7b9b-4a72-9cc6-6cba31ed1275">ITAgentSession</a> interface.


### -param pceltFetched [out]

Pointer to number of elements actually supplied. May be <b>NULL</b> if <i>celt</i> is one.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Method returned <i>celt</i> number of elements.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
Number of elements remaining was less than <i>celt</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppElements</i> parameter is not a valid pointer.

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
 




## -remarks



TAPI calls the <b>AddRef</b> method on the 
<a href="https://msdn.microsoft.com/b0db0834-7b9b-4a72-9cc6-6cba31ed1275">ITAgentSession</a> interface returned by <b>IEnumAgentSession::Next</b>. The application must call <b>Release</b> on the 
<b>ITAgentSession</b> interface to free resources associated with it.




## -see-also




<a href="https://msdn.microsoft.com/38b9fc57-a0af-4dfa-9058-e721138c8be9">IEnumAgentSession</a>



<a href="https://msdn.microsoft.com/b0db0834-7b9b-4a72-9cc6-6cba31ed1275">ITAgentSession</a>
 

 

