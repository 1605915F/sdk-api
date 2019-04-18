---
UID: NF:austream.IAudioData.SetFormat
title: IAudioData::SetFormat (austream.h)
author: windows-sdk-content
description: Note  This interface is deprecated. New applications should not use it. The SetFormat method sets the current data format.
old-location: dshow\iaudiodata_setformat.htm
tech.root: DirectShow
ms.assetid: 792112a6-b10a-432f-854a-07bd74173e84
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IAudioData interface [DirectShow],SetFormat method, IAudioData.SetFormat, IAudioData::SetFormat, IAudioDataSetFormat, SetFormat, SetFormat method [DirectShow], SetFormat method [DirectShow],IAudioData interface, austream/IAudioData::SetFormat, dshow.iaudiodata_setformat
ms.topic: method
req.header: austream.h
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
 - austream.h
api_name:
 - IAudioData.SetFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAudioData::SetFormat


## -description



<div class="alert"><b>Note</b>  This interface is deprecated. New applications should not use it.</div>
<div> </div>
The <code>SetFormat</code> method sets the current data format.




## -parameters




### -param lpWaveFormat [in]

Pointer to a <a href="https://msdn.microsoft.com/4f3bf6fb-b15f-43b3-82f1-e7a8a3007057">WAVEFORMATEX</a> structure that will contain the current data format.


## -returns



Returns an <b>HRESULT</b> value, which can include the following values.

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
Invalid pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid format.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd389513(v=VS.85).aspx">IAudioData Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd389514(v=VS.85).aspx">IAudioData::GetFormat</a>
 

 

