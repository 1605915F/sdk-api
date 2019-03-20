---
UID: NF:vmr9.IVMRImageCompositor9.TermCompositionDevice
title: IVMRImageCompositor9::TermCompositionDevice (vmr9.h)
author: windows-sdk-content
description: The TermCompositionDevice method informs the compositor that the current composition target is being replaced. Compositors should perform any necessary cleanup of the composition target in this method.
old-location: dshow\ivmrimagecompositor9_termcompositiondevice.htm
tech.root: DirectShow
ms.assetid: e218222b-fed3-4f4b-8d97-785774800d89
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVMRImageCompositor9 interface [DirectShow],TermCompositionDevice method, IVMRImageCompositor9.TermCompositionDevice, IVMRImageCompositor9::TermCompositionDevice, IVMRImageCompositor9TermCompositionDevice, TermCompositionDevice, TermCompositionDevice method [DirectShow], TermCompositionDevice method [DirectShow],IVMRImageCompositor9 interface, dshow.ivmrimagecompositor9_termcompositiondevice, vmr9/IVMRImageCompositor9::TermCompositionDevice
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
 - IVMRImageCompositor9.TermCompositionDevice
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVMRImageCompositor9::TermCompositionDevice


## -description



The <code>TermCompositionDevice</code> method informs the compositor that the current composition target is being replaced. Compositors should perform any necessary cleanup of the composition target in this method.




## -parameters




### -param pD3DDevice [in]

Pointer to the <b>IUnknown</b> interface of the Direct3D device object.


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
</table>
 




## -remarks



Include DShow.h and D3d9.h before Vmr9.h.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd377381(v=VS.85).aspx">IVMRImageCompositor9 Interface</a>



<a href="https://msdn.microsoft.com/3d0fdfac-ec7e-4e02-886b-2039c607dac7">Using the Video Mixing Renderer</a>
 

 

