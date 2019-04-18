---
UID: NF:wmcodecdsp.IToc.SetDescriptor
title: IToc::SetDescriptor (wmcodecdsp.h)
author: windows-sdk-content
description: The SetDescriptor method associates a descriptor with the table of contents.
old-location: mf\itoc_setdescriptor.htm
tech.root: medfound
ms.assetid: 55208226-fd2d-48e5-887b-34e95309a770
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IToc interface [Media Foundation],SetDescriptor method, IToc.SetDescriptor, IToc::SetDescriptor, SetDescriptor, SetDescriptor method [Media Foundation], SetDescriptor method [Media Foundation],IToc interface, codecapi.itoc_setdescriptor, mf.itoc_setdescriptor, wmcodecdsp/IToc::SetDescriptor
ms.topic: method
req.header: wmcodecdsp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: Wmvdspa.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmvdspa.dll
api_name:
 - IToc.SetDescriptor
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IToc::SetDescriptor


## -description


The <b>SetDescriptor</b> method associates a descriptor with the table of contents.


## -parameters




### -param pDescriptor [in]

Pointer to a <a href="https://msdn.microsoft.com/a79f75c5-be98-4120-85be-71bedbcc0ea2">TOC_DESCRIPTOR</a> structure that contains the descriptor.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

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
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/4568b50f-a777-4c3d-8c71-66737d24b7cd">GetDescriptor</a>



<a href="https://msdn.microsoft.com/b12d38c7-b80e-4ca8-9ac5-a116100911d0">IToc</a>
 

 

