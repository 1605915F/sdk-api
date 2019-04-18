---
UID: NF:vmr9.IVMRFilterConfig9.SetRenderingMode
title: IVMRFilterConfig9::SetRenderingMode (vmr9.h)
author: windows-sdk-content
description: The SetRenderingMode method sets the rendering mode used by the VMR.
old-location: dshow\ivmrfilterconfig9_setrenderingmode.htm
tech.root: DirectShow
ms.assetid: d7a27d7c-5cd4-4a20-ba15-7056d502e3e3
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVMRFilterConfig9 interface [DirectShow],SetRenderingMode method, IVMRFilterConfig9.SetRenderingMode, IVMRFilterConfig9::SetRenderingMode, IVMRFilterConfig9SetRenderingMode, SetRenderingMode, SetRenderingMode method [DirectShow], SetRenderingMode method [DirectShow],IVMRFilterConfig9 interface, dshow.ivmrfilterconfig9_setrenderingmode, vmr9/IVMRFilterConfig9::SetRenderingMode
ms.topic: method
req.header: vmr9.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IVMRFilterConfig9.SetRenderingMode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVMRFilterConfig9::SetRenderingMode


## -description



The <code>SetRenderingMode</code> method sets the rendering mode used by the VMR.




## -parameters




### -param Mode [in]

Specifies the rendering mode as a <a href="https://msdn.microsoft.com/en-us/library/Dd407367(v=VS.85).aspx">VMR9Mode</a> value.


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
An invalid rendering mode was specified.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VFW_E_WRONG_STATE</b></dt>
</dl>
</td>
<td width="60%">
The mode cannot be changed for some reason. See Remarks.

</td>
</tr>
</table>
 




## -remarks



The VMR is in windowed mode (<b>VMR9Mode_Windowed</b>) by default. Use this method to put the VMR into windowless mode (<b>VMR9Mode_Windowless</b>) or renderless mode (<b>VMR9Mode_Renderless</b>).

The mode cannot be changed after any pin has been connected. Also, the mode cannot be changed from windowless or renderless mode back to windowed mode, even before pins are connected. Therefore, specifying <b>VMR9Mode_Windowed</b> for the <i>Mode</i> parameter has no effect under any circumstances.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd377365(v=VS.85).aspx">IVMRFilterConfig9 Interface</a>



<a href="https://msdn.microsoft.com/3d0fdfac-ec7e-4e02-886b-2039c607dac7">Using the Video Mixing Renderer</a>



<a href="https://msdn.microsoft.com/98244af1-5934-4d1c-b9c3-7a414b065fe7">VMR Modes of Operation</a>
 

 

