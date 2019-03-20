---
UID: NF:winsync.ISyncKnowledge2.GetIdParameters
title: ISyncKnowledge2::GetIdParameters (winsync.h)
author: windows-sdk-content
description: Gets the ID format schema of the provider.
old-location: winsync\isyncknowledge2_getidparameters.htm
tech.root: winsync
ms.assetid: dbb049b8-cd2c-49f3-a9f9-0d76da0b3824
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetIdParameters, GetIdParameters method [Windows Sync], GetIdParameters method [Windows Sync],ISyncKnowledge2 interface, ISyncKnowledge2 interface [Windows Sync],GetIdParameters method, ISyncKnowledge2.GetIdParameters, ISyncKnowledge2::GetIdParameters, winsync.isyncknowledge2_getidparameters, winsync/ISyncKnowledge2::GetIdParameters
ms.topic: method
req.header: winsync.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - winsync.h
api_name:
 - ISyncKnowledge2.GetIdParameters
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISyncKnowledge2::GetIdParameters


## -description


Gets the ID format schema of the provider.


## -parameters




### -param pIdParameters [out]

The ID format schema of the provider.


## -returns



The possible return codes include, but are not limited to, the values shown in the following table.

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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>dwSize</i> member of <i>pIdParameters</i> is not equal to <code>sizeof(ID_PARAMETERS)</code>.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
Invalid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/cfb08476-7b5d-4953-b723-5160330e57be">ISyncKnowledge Interface</a>



<a href="https://msdn.microsoft.com/1acbae32-8fa6-4c1e-95f6-30aca483c966">ISyncKnowledge2 Interface</a>
 

 

