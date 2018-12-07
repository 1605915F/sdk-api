---
UID: NF:mstask.IEnumWorkItems.Skip
title: IEnumWorkItems::Skip
author: windows-sdk-content
description: Skips the next specified number of tasks in the enumeration sequence.
old-location: taskschd\ienumworkitems_skip.htm
tech.root: taskschd
ms.assetid: 5f4c7c98-a802-4fc3-b88f-bb37826f8199
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumWorkItems interface [Task Scheduler],Skip method, IEnumWorkItems.Skip, IEnumWorkItems::Skip, Skip, Skip method [Task Scheduler], Skip method [Task Scheduler],IEnumWorkItems interface, _msb_ienumworkitems_skip, mstask/IEnumWorkItems::Skip, taskschd.ienumworkitems_skip
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mstask.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mstask.lib
req.dll: Mstask.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mstask.dll
api_name:
 - IEnumWorkItems.Skip
product: Windows
targetos: Windows
req.typenames: 
req.redist: Internet Explorer 4.0 or later on Windows NT 4.0 and Windows 95
---

# IEnumWorkItems::Skip


## -description


<p class="CCE_Message">[[This API may be altered or unavailable in subsequent versions of the operating system or product. Please use the <a href="https://msdn.microsoft.com/67ed58e1-e54c-4c02-a6c4-d9ab8dc0f83e">Task Scheduler 2.0 Interfaces</a> instead.] ]

Skips the next specified number of tasks in the enumeration sequence.




## -parameters




### -param celt [in]

The number of tasks to be skipped.


## -returns



Returns one of the following values.

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
The number of elements skipped equals <i>celt</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The number of elements remaining in the sequence is less than the value specified in <i>celt</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The value of <i>celt</i> is less than or equal to zero.

</td>
</tr>
</table>
 




## -remarks



The 
<a href="https://msdn.microsoft.com/1af162e5-8ba1-4d2e-9451-39c80ac0eecf">IEnumWorkItems</a> interface also provides methods for retrieving sets of tasks, resetting the enumeration sequence, and making a copy of the current state of the enumeration.




## -see-also




<a href="https://msdn.microsoft.com/1af162e5-8ba1-4d2e-9451-39c80ac0eecf">IEnumWorkItems</a>



<a href="https://msdn.microsoft.com/c42550df-33ad-49cc-ab89-5f952cce2a83">IEnumWorkItems::Clone</a>



<a href="https://msdn.microsoft.com/a606e340-33fb-4a51-acdd-b7428c755ac5">IEnumWorkItems::Next</a>



<a href="https://msdn.microsoft.com/920ba47b-41cd-462b-9b72-73898a5cd4d0">IEnumWorkItems::Reset</a>
 

 

