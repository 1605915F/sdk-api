---
UID: NF:d3d10.ID3D10Texture1D.Unmap
title: ID3D10Texture1D::Unmap (d3d10.h)
author: windows-sdk-content
description: Invalidate the pointer to a resource that was retrieved by ID3D10Texture1D::Map, and re-enable the GPU's access to that resource.
old-location: direct3d10\id3d10texture1d_unmap.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10texture1d_unmap.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 19252c0c-8539-ab86-d402-c4d9d235f30e, ID3D10Texture1D interface [Direct3D 10],Unmap method, ID3D10Texture1D.Unmap, ID3D10Texture1D::Unmap, Unmap, Unmap method [Direct3D 10], Unmap method [Direct3D 10],ID3D10Texture1D interface, d3d10/ID3D10Texture1D::Unmap, direct3d10.id3d10texture1d_unmap
ms.topic: method
req.header: d3d10.h
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
req.lib: D3D10.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D10.lib
 - D3D10.dll
api_name:
 - ID3D10Texture1D.Unmap
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10Texture1D::Unmap


## -description


Invalidate the pointer to a resource that was retrieved by <a href="https://msdn.microsoft.com/en-us/library/Bb173865(v=VS.85).aspx">ID3D10Texture1D::Map</a>, and re-enable the GPU's access to that resource.


## -parameters




### -param Subresource [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb205133(v=VS.85).aspx">Subresource</a> to be unmapped. See <a href="https://msdn.microsoft.com/en-us/library/Bb694525(v=VS.85).aspx">D3D10CalcSubresource</a> for more details.


## -returns



Returns nothing.




## -remarks



A subresource must be mapped before Unmap is called.

<table>
<tr>
<td>
Differences between Direct3D 9 and Direct3D 10:

Unmap in Direct3D 10 is analogous to resource Unlock in Direct3D 9.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173863(v=VS.85).aspx">ID3D10Texture1D Interface</a>
 

 

