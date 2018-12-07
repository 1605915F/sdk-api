---
UID: NF:atscpsipparser.IAtscPsipParser.GetPMT
title: IAtscPsipParser::GetPMT
author: windows-sdk-content
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
old-location: mstv\iatscpsipparser_getpmt.htm
tech.root: mstv
ms.assetid: cd9a3fb0-4bdc-499b-9db9-85dce50dd24b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPMT, GetPMT method [Microsoft TV Technologies], GetPMT method [Microsoft TV Technologies],IAtscPsipParser interface, IAtscPsipParser interface [Microsoft TV Technologies],GetPMT method, IAtscPsipParser.GetPMT, IAtscPsipParser::GetPMT, IAtscPsipParserGetPMT, atscpsipparser/IAtscPsipParser::GetPMT, mstv.iatscpsipparser_getpmt
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IAtscPsipParser.GetPMT
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAtscPsipParser::GetPMT


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>GetPMT</b> method retrieves the program map table (PMT) for a specified packet identifier (PID).


## -parameters




### -param pid [in]

Specifies the PID for the requested PMT.


### -param pwProgramNumber [in]

Optional pointer to a variable that contains a table program number. You can use this value to filter the request. Otherwise, set this parameter to <b>NULL</b>.


### -param ppPMT [out]

Receives an <a href="https://msdn.microsoft.com/0dbd4cc3-5ef3-4c71-ba3f-149d5050ba24">IPMT</a> interface pointer. The caller must release the interface.


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
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<b>NULL</b> pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_SECTION_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The filter did not receive the table in the allotted time.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_UNINITIALIZED</b></dt>
</dl>
</td>
<td width="60%">
The <b>Initialize</b> method was not called.

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
 




## -remarks



The method fails if the filter does not receive a matching table within a predetermined length of time.




## -see-also




<a href="https://msdn.microsoft.com/dbe922b3-b843-4eaa-807d-5608cfbb9686">IAtscPsipParser Interface</a>
 

 

