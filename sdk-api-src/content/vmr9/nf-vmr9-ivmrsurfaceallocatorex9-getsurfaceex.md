---
UID: NF:vmr9.IVMRSurfaceAllocatorEx9.GetSurfaceEx
title: IVMRSurfaceAllocatorEx9::GetSurfaceEx (vmr9.h)
author: windows-sdk-content
description: The GetSurfaceEx method retrieves a Direct3D surface and a destination rectangle.
old-location: dshow\ivmrsurfaceallocatorex9_getsurfaceex.htm
tech.root: DirectShow
ms.assetid: 828f1ea6-4093-4a33-bc41-0f6fff752bcf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetSurfaceEx, GetSurfaceEx method [DirectShow], GetSurfaceEx method [DirectShow],IVMRSurfaceAllocatorEx9 interface, IVMRSurfaceAllocatorEx9 interface [DirectShow],GetSurfaceEx method, IVMRSurfaceAllocatorEx9.GetSurfaceEx, IVMRSurfaceAllocatorEx9::GetSurfaceEx, IVMRSurfaceAllocatorEx9GetSurfaceEx, dshow.ivmrsurfaceallocatorex9_getsurfaceex, vmr9/IVMRSurfaceAllocatorEx9::GetSurfaceEx
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
 - IVMRSurfaceAllocatorEx9.GetSurfaceEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVMRSurfaceAllocatorEx9::GetSurfaceEx


## -description


The <b>GetSurfaceEx</b> method retrieves a Direct3D surface and a destination rectangle.


## -parameters




### -param dwUserID [in]

Application-defined identifier. This value is the same value that the application passed to the <a href="https://msdn.microsoft.com/en-us/library/Dd390509(v=VS.85).aspx">IVMRSurfaceAllocatorNotify9::AdviseSurfaceAllocator</a> method in the <i>dwUserID</i> parameter..


### -param SurfaceIndex [in]

Index of the surface to retrieve.


### -param SurfaceFlags [in]

Surface flags.


### -param lplpSurface [out]

Receives a pointer to the <b>IDirect3DSurface9</b> interface. The caller must release the interface.


### -param lprcDst [out]

Location within the surface where the VMR-9 should write the composited image.


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




<a href="https://msdn.microsoft.com/en-us/library/Dd390505(v=VS.85).aspx">IVMRSurfaceAllocatorEx9 Interface</a>



<a href="https://msdn.microsoft.com/3d0fdfac-ec7e-4e02-886b-2039c607dac7">Using the Video Mixing Renderer</a>
 

 

