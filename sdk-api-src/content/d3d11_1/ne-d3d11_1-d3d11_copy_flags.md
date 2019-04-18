---
UID: NE:d3d11_1.D3D11_COPY_FLAGS
title: D3D11_COPY_FLAGS (d3d11_1.h)
author: windows-sdk-content
description: Specifies how to handle the existing contents of a resource during a copy or update operation of a region within that resource.
old-location: direct3d11\d3d11_copy_flags.htm
tech.root: direct3d11
ms.assetid: 2141A053-931B-42F2-BC8C-AAE9F4739ED7
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: D3D11_COPY_DISCARD, D3D11_COPY_FLAGS, D3D11_COPY_FLAGS enumeration [Direct3D 11], D3D11_COPY_NO_OVERWRITE, d3d11_1/D3D11_COPY_DISCARD, d3d11_1/D3D11_COPY_FLAGS, d3d11_1/D3D11_COPY_NO_OVERWRITE, direct3d11.d3d11_copy_flags
ms.topic: enum
req.header: d3d11_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps only]
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
 - HeaderDef
api_location:
 - D3D11_1.h
api_name:
 - D3D11_COPY_FLAGS
product: Windows
targetos: Windows
req.typenames: D3D11_COPY_FLAGS
req.redist: 
ms.custom: 19H1
---

# D3D11_COPY_FLAGS enumeration


## -description


<div class="alert"><b>Note</b>  This enumeration is supported by the Direct3D 11.1 runtime, which is available on Windows 8 and later operating systems.</div><div> </div>Specifies how to handle the existing contents of a resource during a copy or update operation of a region within that resource.


## -enum-fields




### -field D3D11_COPY_NO_OVERWRITE

The existing contents of the resource cannot be overwritten.


### -field D3D11_COPY_DISCARD

The existing contents of the resource are undefined and can be discarded.


## -see-also




<a href="https://msdn.microsoft.com/1641713a-5ac8-4597-900b-1bba54f9f522">Core Enumerations</a>



<a href="https://msdn.microsoft.com/1963011F-C3E2-428D-B667-195A4976510B">ID3D11DeviceContext1::CopySubresourceRegion1</a>



<a href="https://msdn.microsoft.com/7D89591C-F3F7-4A4F-A91A-AC67D9A573AF">ID3D11DeviceContext1::UpdateSubresource1</a>
 

 

