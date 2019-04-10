---
UID: NF:tapi3if.ITForwardInformation.get_NumRingsNoAnswer
title: ITForwardInformation::get_NumRingsNoAnswer (tapi3if.h)
author: windows-sdk-content
description: The get_NumRingsNoAnswer method retrieves the number of rings after which a no answer condition is assumed.
old-location: tapi3\itforwardinformation_get_numringsnoanswer.htm
tech.root: Tapi
ms.assetid: bfd46f8b-6501-43ca-b3bd-35394526d5ce
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITForwardInformation interface [TAPI 2.2],get_NumRingsNoAnswer method, ITForwardInformation.get_NumRingsNoAnswer, ITForwardInformation::get_NumRingsNoAnswer, _tapi3_itforwardinformation_get_numringsnoanswer, get_NumRingsNoAnswer, get_NumRingsNoAnswer method [TAPI 2.2], get_NumRingsNoAnswer method [TAPI 2.2],ITForwardInformation interface, tapi3.itforwardinformation_get_numringsnoanswer, tapi3if/ITForwardInformation::get_NumRingsNoAnswer
ms.topic: method
req.header: tapi3if.h
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
 - ITForwardInformation.get_NumRingsNoAnswer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITForwardInformation::get_NumRingsNoAnswer


## -description


The 
<b>get_NumRingsNoAnswer</b> method retrieves the number of rings after which a no answer condition is assumed.


## -parameters




### -param plNumRings [out]

Pointer to number of rings.


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
Method succeeded.

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
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>plNumRings</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/87d37ba3-5398-47a7-808b-eb9b6681653d">ITAddress::CreateForwardInfoObject</a>



<a href="https://msdn.microsoft.com/4f070b50-db9a-49e8-a0f3-e448c5dee144">ITAddress::Forward</a>



<a href="https://msdn.microsoft.com/7817ac03-d9fc-4042-ae7d-350ee6cbef53">ITAddress::get_CurrentForwardInfo</a>



<a href="https://msdn.microsoft.com/0e06cd0b-b95b-4853-b883-53146be084f0">ITForwardInformation</a>



<a href="https://msdn.microsoft.com/0d96f229-76c0-46a3-bc4b-6f558b9956c6">Terminal Object</a>



<a href="https://msdn.microsoft.com/ad7b2746-cb97-406e-a328-efc051681aa6">put_NumRingsNoAnswer</a>
 

 

