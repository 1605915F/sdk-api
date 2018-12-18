---
UID: NF:atscpsipparser.IATSC_EIT.GetProtocolVersion
title: IATSC_EIT::GetProtocolVersion
author: windows-sdk-content
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
old-location: mstv\iatsc_eit_getprotocolversion.htm
tech.root: mstv
ms.assetid: fa1234b4-8976-404c-b27d-320d2bba5794
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetProtocolVersion, GetProtocolVersion method [Microsoft TV Technologies], GetProtocolVersion method [Microsoft TV Technologies],IATSC_EIT interface, IATSC_EIT interface [Microsoft TV Technologies],GetProtocolVersion method, IATSC_EIT.GetProtocolVersion, IATSC_EIT::GetProtocolVersion, IATSC_EITGetProtocolVersion, atscpsipparser/IATSC_EIT::GetProtocolVersion, mstv.iatsc_eit_getprotocolversion
ms.topic: method
req.header: atscpsipparser.h
req.include-header: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - atscpsipparser.h
api_name:
 - IATSC_EIT.GetProtocolVersion
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IATSC_EIT::GetProtocolVersion


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>GetProtocolVersion</b> method returns the protocol version of the table.


## -parameters




### -param pbVal [out]

Receives the protocol_version field.


## -returns



The method returns an <b>HRESULT</b>. Possible values include those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
NULL pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/ab3fd79f-4ca6-418e-8e7c-a5fa196c09e6">IATSC_EIT Interface</a>
 

 

