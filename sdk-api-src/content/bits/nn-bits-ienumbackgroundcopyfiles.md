---
UID: NN:bits.IEnumBackgroundCopyFiles
title: IEnumBackgroundCopyFiles
author: windows-sdk-content
description: Use the IEnumBackgroundCopyFiles interface to enumerate the files that a job contains. To get an IEnumBackgroundCopyFiles interface pointer, call the IBackgroundCopyJob::EnumFiles method.
old-location: bits\ienumbackgroundcopyfiles.htm
tech.root: Bits
ms.assetid: 831998ba-601c-43c4-ba27-faff741f8eb4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumBackgroundCopyFiles, IEnumBackgroundCopyFiles interface [BITS], IEnumBackgroundCopyFiles interface [BITS],described, _drz_ienumbackgroundcopyfiles, bits.ienumbackgroundcopyfiles, bits/IEnumBackgroundCopyFiles
ms.topic: interface
req.header: bits.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Bits.lib
req.dll: QmgrPrxy.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - QmgrPrxy.dll
api_name:
 - IEnumBackgroundCopyFiles
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumBackgroundCopyFiles interface


## -description


Use the 
<b>IEnumBackgroundCopyFiles</b> interface to enumerate the files that a job contains. To get an 
<b>IEnumBackgroundCopyFiles</b> interface pointer, call the 
<a href="https://msdn.microsoft.com/c6b8ef69-9c67-447f-9f90-b6905a5a5a19">IBackgroundCopyJob::EnumFiles</a> method.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumBackgroundCopyFiles</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IEnumBackgroundCopyFiles</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEnumBackgroundCopyFiles</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ea2d2f76-7cd9-4e48-8a2c-3dd367afdee7">Clone</a>
</td>
<td align="left" width="63%">
Creates another enumerator that contains the same enumeration state as the current enumerator.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/24a9d5f9-e923-4b20-8abf-8ce50fc2602b">GetCount</a>
</td>
<td align="left" width="63%">
Retrieves the number of items in the enumeration.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ac62533a-8949-41b9-a3e6-f9030884a9ce">Next</a>
</td>
<td align="left" width="63%">
Retrieves a specified number of items in the enumeration sequence.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/471e1417-8d22-4368-93f4-151aa8a662ba">Reset</a>
</td>
<td align="left" width="63%">
Resets the enumeration sequence to the beginning.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/41488586-cb91-4b87-b11d-2808bc162d42">Skip</a>
</td>
<td align="left" width="63%">
Skips a specified number of items in the enumeration sequence.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/c6b8ef69-9c67-447f-9f90-b6905a5a5a19">IBackgroundCopyJob::EnumFiles</a>



<a href="https://msdn.microsoft.com/21ff88da-9fae-478f-bcba-488ed7a89608">IEnumBackgroundCopyJobs</a>
 

 

