---
UID: NF:d3d11sdklayers.ID3D11Debug.GetSwapChain
title: ID3D11Debug::GetSwapChain (d3d11sdklayers.h)
author: windows-sdk-content
description: Get the swap chain that the runtime will use for automatically calling IDXGISwapChain::Present.
old-location: direct3d11\id3d11debug_getswapchain.htm
tech.root: direct3d11
ms.assetid: 99dcdddf-dec8-497e-862a-72ef66528fa5
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSwapChain, GetSwapChain method [Direct3D 11], GetSwapChain method [Direct3D 11],ID3D11Debug interface, ID3D11Debug interface [Direct3D 11],GetSwapChain method, ID3D11Debug.GetSwapChain, ID3D11Debug::GetSwapChain, c20306ae-8125-a9ff-0c0f-c8368ec1b294, d3d11sdklayers/ID3D11Debug::GetSwapChain, direct3d11.id3d11debug_getswapchain
ms.topic: method
req.header: d3d11sdklayers.h
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
 - ID3D11Debug.GetSwapChain
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D11Debug::GetSwapChain


## -description


Get the swap chain that the runtime will use for automatically calling <a href="https://msdn.microsoft.com/en-us/library/Bb174576(v=VS.85).aspx">IDXGISwapChain::Present</a>.


## -parameters




### -param ppSwapChain [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb174569(v=VS.85).aspx">IDXGISwapChain</a>**</b>

Swap chain that the runtime will use for automatically calling <a href="https://msdn.microsoft.com/en-us/library/Bb174576(v=VS.85).aspx">IDXGISwapChain::Present</a>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the following <a href="https://msdn.microsoft.com/c0856a58-b760-44e5-8acf-145720b403d1">Direct3D 11 Return Codes</a>.




## -remarks



The swap chain retrieved by this method will only be used if D3D11_DEBUG_FEATURE_PRESENT_PER_RENDER_OP is set in the <a href="https://msdn.microsoft.com/60f9da61-dc97-4b6d-b187-df3605ad9336">feature mask</a>.




## -see-also




<a href="https://msdn.microsoft.com/2c640295-7a91-4a7a-92d3-909d288eb0d6">ID3D11Debug Interface</a>
 

 

