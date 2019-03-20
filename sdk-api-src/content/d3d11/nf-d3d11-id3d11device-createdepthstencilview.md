---
UID: NF:d3d11.ID3D11Device.CreateDepthStencilView
title: ID3D11Device::CreateDepthStencilView (d3d11.h)
author: windows-sdk-content
description: Create a depth-stencil view for accessing resource data.
old-location: direct3d11\id3d11device_createdepthstencilview.htm
tech.root: direct3d11
ms.assetid: b3e899eb-3df6-421f-bdc8-98d7c7acbe62
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateDepthStencilView, CreateDepthStencilView method [Direct3D 11], CreateDepthStencilView method [Direct3D 11],ID3D11Device interface, ID3D11Device interface [Direct3D 11],CreateDepthStencilView method, ID3D11Device.CreateDepthStencilView, ID3D11Device::CreateDepthStencilView, d3d11/ID3D11Device::CreateDepthStencilView, direct3d11.id3d11device_createdepthstencilview, e1e786e8-1374-b092-ac91-06c2482f6166
ms.topic: method
req.header: d3d11.h
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
req.lib: D3D11.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D11.lib
 - D3D11.dll
api_name:
 - ID3D11Device.CreateDepthStencilView
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11Device::CreateDepthStencilView


## -description


Create a depth-stencil view for accessing resource data.


## -parameters




### -param pResource [in]

Type: <b><a href="https://msdn.microsoft.com/3823ec00-cb3c-43ce-9f1a-be4e1e99d587">ID3D11Resource</a>*</b>

Pointer to the resource that will serve as the depth-stencil surface. This resource must have been created with the <a href="https://msdn.microsoft.com/4ffa1714-bd85-4d5a-930d-20526f46e4b9">D3D11_BIND_DEPTH_STENCIL</a> flag.


### -param pDesc [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/f073a798-edd5-4e6a-a8a7-1592721ce35d">D3D11_DEPTH_STENCIL_VIEW_DESC</a>*</b>

Pointer to a depth-stencil-view description (see <a href="https://msdn.microsoft.com/f073a798-edd5-4e6a-a8a7-1592721ce35d">D3D11_DEPTH_STENCIL_VIEW_DESC</a>). Set this parameter to <b>NULL</b> to create a view that accesses mipmap level 0 of the entire resource (using the format the resource was created with).


### -param ppDepthStencilView [out, optional]

Type: <b><a href="https://msdn.microsoft.com/10be1fd1-8700-4c0a-b447-d3c2569f8e81">ID3D11DepthStencilView</a>**</b>

Address of a pointer to an <a href="https://msdn.microsoft.com/10be1fd1-8700-4c0a-b447-d3c2569f8e81">ID3D11DepthStencilView</a>. Set this parameter to <b>NULL</b> to validate the other input parameters (the method will return S_FALSE if the other input parameters pass validation).


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the following <a href="https://msdn.microsoft.com/c0856a58-b760-44e5-8acf-145720b403d1">Direct3D 11 Return Codes</a>.




## -remarks



A depth-stencil view can be bound to the output-merger stage by calling <a href="https://msdn.microsoft.com/65514812-7433-4c13-a6cb-53980dacdf65">ID3D11DeviceContext::OMSetRenderTargets</a>.




## -see-also




<a href="https://msdn.microsoft.com/2f2559d9-1cd6-44f6-90e2-ee0f86e39f78">ID3D11Device</a>
 

 

