---
UID: NF:tom.ITextStrings.SuffixTop
title: ITextStrings::SuffixTop (tom.h)
author: windows-sdk-content
description: Suffixes a string to the top string in the collection.
old-location: controls\itextstrings_suffixtop.htm
tech.root: Controls
ms.assetid: 66f4e5c6-e97b-48a5-9c71-3efb1eba12d6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITextStrings interface [Windows Controls],SuffixTop method, ITextStrings.SuffixTop, ITextStrings::SuffixTop, SuffixTop, SuffixTop method [Windows Controls], SuffixTop method [Windows Controls],ITextStrings interface, controls.itextstrings_suffixtop, tom/ITextStrings::SuffixTop
ms.topic: method
req.header: tom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextStrings.SuffixTop
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextStrings::SuffixTop


## -description


Suffixes a string to the top string in the collection. 


## -parameters




### -param bstr [in]

Type: <b>BSTR</b>

The text to suffix to the top string.


### -param pRange [in]

Type: <b><a href="https://msdn.microsoft.com/905f0967-8b99-45ed-a1cc-19d49e919a65">ITextRange2</a>*</b>

The range with the desired character formatting.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the method succeeds, it returns <b>S_OK</b>. If the method fails, it returns one of the following COM error codes. For more information about COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.

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
</table>
 




## -remarks



This method is similar to <a href="https://msdn.microsoft.com/e280008b-b41e-43e3-9f16-6fe1f88e10ea">ITextStrings::Append</a>, but appends a string instead of a range.




## -see-also




<a href="https://msdn.microsoft.com/c878d0db-ac13-4ac9-8601-d1c1ba76cd85">ITextStrings</a>
 

 

