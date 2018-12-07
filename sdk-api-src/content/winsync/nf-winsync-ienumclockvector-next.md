---
UID: NF:winsync.IEnumClockVector.Next
title: IEnumClockVector::Next
author: windows-sdk-content
description: Returns the next elements in the clock vector, if they are available.
old-location: winsync\ienumclockvector_next.htm
tech.root: winsync
ms.assetid: 40aa741a-b536-4a8b-9f97-b7b599e49aef
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumClockVector interface [Windows Sync],Next method, IEnumClockVector.Next, IEnumClockVector::Next, Next, Next method [Windows Sync], Next method [Windows Sync],IEnumClockVector interface, winsync.ienumclockvector_next, winsync/IEnumClockVector::Next
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IEnumClockVector.Next
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumClockVector::Next


## -description


Returns the next elements in the clock vector, if they are available.


## -parameters




### -param cClockVectorElements [in]

The number of clock vector elements to retrieve in the range of zero to 1000.


### -param ppiClockVectorElements [out]

Returns the next <i>pcFetched</i> clock vector elements.



### -param pcFetched [in, out]

Returns the number of clock vector elements that were retrieved. This value can be <b>NULL</b> if <i>cClockVectorElements</i> is 1; otherwise, it cannot be <b>NULL</b>.


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
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
If there are no more elements to retrieve.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%"></td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/cf191502-dc51-44a7-a82f-a0e38537574f">IEnumClockVector Interface</a>
 

 

