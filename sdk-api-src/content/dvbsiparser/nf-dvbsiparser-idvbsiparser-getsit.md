---
UID: NF:dvbsiparser.IDvbSiParser.GetSIT
title: IDvbSiParser::GetSIT
author: windows-sdk-content
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
old-location: mstv\idvbsiparser_getsit.htm
tech.root: mstv
ms.assetid: d316858e-8014-499c-9727-0a839658fa18
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetSIT, GetSIT method [Microsoft TV Technologies], GetSIT method [Microsoft TV Technologies],IDvbSiParser interface, IDvbSiParser interface [Microsoft TV Technologies],GetSIT method, IDvbSiParser.GetSIT, IDvbSiParser::GetSIT, IDvbSiParserGetSIT, dvbsiparser/IDvbSiParser::GetSIT, mstv.idvbsiparser_getsit
ms.topic: method
req.header: dvbsiparser.h
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
 - dvbsiparser.h
api_name:
 - IDvbSiParser.GetSIT
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDvbSiParser::GetSIT


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>GetSIT</b> method retrieves the selection information table (SIT).


## -parameters




### -param dwTimeout [in]

Specifies a time-out value, in milliseconds. If the filter does not receive the data within the time-out period, the method fails.


### -param ppSIT [out]

Address of a variable that receives an <a href="https://msdn.microsoft.com/f278d942-a450-4a01-998d-4dac1c8a1fcc">IDVB_SIT</a> interface pointer. The caller must release the interface.


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
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/092162af-5f88-4ce5-ac2f-89327f094804">IDvbSiParser Interface</a>
 

 

