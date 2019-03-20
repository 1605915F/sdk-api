---
UID: NF:winsync.ISyncKnowledge2.CompareToKnowledgeCookie
title: ISyncKnowledge2::CompareToKnowledgeCookie (winsync.h)
author: windows-sdk-content
description: Performs a fast comparison between the specified knowledge cookie and this knowledge object.
old-location: winsync\isyncknowledge2_comparetoknowledgecookie.htm
tech.root: winsync
ms.assetid: f1649f70-8c8b-4eea-8ecb-7ea5a657eabe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CompareToKnowledgeCookie, CompareToKnowledgeCookie method [Windows Sync], CompareToKnowledgeCookie method [Windows Sync],ISyncKnowledge2 interface, ISyncKnowledge2 interface [Windows Sync],CompareToKnowledgeCookie method, ISyncKnowledge2.CompareToKnowledgeCookie, ISyncKnowledge2::CompareToKnowledgeCookie, winsync.isyncknowledge2_comparetoknowledgecookie, winsync/ISyncKnowledge2::CompareToKnowledgeCookie
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
 - ISyncKnowledge2.CompareToKnowledgeCookie
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISyncKnowledge2::CompareToKnowledgeCookie


## -description


Performs a fast comparison between the specified knowledge cookie and this knowledge object.



## -parameters




### -param pKnowledgeCookie [in]

The knowledge cookie to compare against this object.


### -param pResult [out]

The result of the comparison.



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
<dt><b>E_POINTER
</b></dt>
</dl>
</td>
<td width="60%">
Invalid pointer.

</td>
</tr>
</table>
 




## -remarks



This method can be used when the performance of the knowledge comparison operation is especially important.





## -see-also




<a href="https://msdn.microsoft.com/cfb08476-7b5d-4953-b723-5160330e57be">ISyncKnowledge Interface</a>



<a href="https://msdn.microsoft.com/1acbae32-8fa6-4c1e-95f6-30aca483c966">ISyncKnowledge2 Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd744812(v=VS.85).aspx">KNOWLEDGE_COOKIE_COMPARISON_RESULT Enumeration</a>
 

 

