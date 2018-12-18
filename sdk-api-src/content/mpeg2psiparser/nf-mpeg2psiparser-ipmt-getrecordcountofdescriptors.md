---
UID: NF:mpeg2psiparser.IPMT.GetRecordCountOfDescriptors
title: IPMT::GetRecordCountOfDescriptors
author: windows-sdk-content
description: The GetRecordCountOfDescriptors method returns the number of descriptors for a record in the PMT.
old-location: mstv\ipmt_getrecordcountofdescriptors.htm
tech.root: mstv
ms.assetid: b2470267-25a6-4ed3-91a1-30fd3ac7bbea
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetRecordCountOfDescriptors, GetRecordCountOfDescriptors method [Microsoft TV Technologies], GetRecordCountOfDescriptors method [Microsoft TV Technologies],IPMT interface, IPMT interface [Microsoft TV Technologies],GetRecordCountOfDescriptors method, IPMT.GetRecordCountOfDescriptors, IPMT::GetRecordCountOfDescriptors, IPMTGetRecordCountOfDescriptors, mpeg2psiparser/IPMT::GetRecordCountOfDescriptors, mstv.ipmt_getrecordcountofdescriptors
ms.topic: method
req.header: mpeg2psiparser.h
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
 - Mpeg2PsiParser.h
api_name:
 - IPMT.GetRecordCountOfDescriptors
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPMT::GetRecordCountOfDescriptors


## -description



The <b>GetRecordCountOfDescriptors</b> method returns the number of descriptors for a record in the PMT.




## -parameters




### -param dwRecordIndex [in]

Specifies the record number, indexed from zero. Call the <a href="https://msdn.microsoft.com/en-us/library/Dd694822(v=VS.85).aspx">IPMT::GetCountOfRecords</a> method to get the number of records in the PMT.


### -param pdwVal [out]

Receives the number of descriptors.


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
<dt><b>MPEG2_E_OUT_OF_BOUNDS</b></dt>
</dl>
</td>
<td width="60%">
Index out of bounds.

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




<a href="https://msdn.microsoft.com/en-us/library/Dd694820(v=VS.85).aspx">IPMT Interface</a>
 

 

