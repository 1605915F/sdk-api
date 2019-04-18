---
UID: NF:strmif.IVMRSurface.UnlockSurface
title: IVMRSurface::UnlockSurface (strmif.h)
author: windows-sdk-content
description: The UnlockSurface method unlocks the attached DirectDraw surface.
old-location: dshow\ivmrsurface_unlocksurface.htm
tech.root: DirectShow
ms.assetid: f6acaf96-925c-46b9-8d56-11d94f3dbda3
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVMRSurface interface [DirectShow],UnlockSurface method, IVMRSurface.UnlockSurface, IVMRSurface::UnlockSurface, IVMRSurfaceUnlockSurface, UnlockSurface, UnlockSurface method [DirectShow], UnlockSurface method [DirectShow],IVMRSurface interface, dshow.ivmrsurface_unlocksurface, strmif/IVMRSurface::UnlockSurface
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - IVMRSurface.UnlockSurface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVMRSurface::UnlockSurface


## -description



The <code>UnlockSurface</code> method unlocks the attached DirectDraw surface.




## -parameters






## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
No DirectDraw surface is attached to this sample.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/8222ea5c-be77-4f33-83ff-073fb3e85e73">IVMRSurface Interface</a>



<a href="https://msdn.microsoft.com/3d0fdfac-ec7e-4e02-886b-2039c607dac7">Using the Video Mixing Renderer</a>
 

 

