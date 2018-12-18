---
UID: NF:dxgi.IDXGISwapChain.GetLastPresentCount
title: IDXGISwapChain::GetLastPresentCount
author: windows-sdk-content
description: Gets the number of times that IDXGISwapChain::Present or IDXGISwapChain1::Present1 has been called.
old-location: direct3ddxgi\idxgiswapchain_getlastpresentcount.htm
tech.root: direct3ddxgi
ms.assetid: VS|directx_sdk|~\idxgiswapchain_getlastpresentcount.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLastPresentCount, GetLastPresentCount method [DXGI], GetLastPresentCount method [DXGI],IDXGISwapChain interface, IDXGISwapChain interface [DXGI],GetLastPresentCount method, IDXGISwapChain.GetLastPresentCount, IDXGISwapChain::GetLastPresentCount, direct3ddxgi.idxgiswapchain_getlastpresentcount, dxgi/IDXGISwapChain::GetLastPresentCount, f6292a4d-50a6-18b3-5edc-a581c15fa784
ms.topic: method
req.header: dxgi.h
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
req.lib: DXGI.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - DXGI.lib
 - DXGI.dll
api_name:
 - IDXGISwapChain.GetLastPresentCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGISwapChain::GetLastPresentCount


## -description


Gets the number of times  that <a href="https://msdn.microsoft.com/en-us/library/Bb174576(v=VS.85).aspx">IDXGISwapChain::Present</a> or <a href="https://msdn.microsoft.com/F795A719-71BA-4A25-B41A-9D93F96B6CA4">IDXGISwapChain1::Present1</a> has been called.


## -parameters




### -param pLastPresentCount [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

A pointer to a variable that receives the number of calls.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns one of the <a href="https://msdn.microsoft.com/en-us/library/Bb509553(v=VS.85).aspx">DXGI_ERROR</a> values.




## -remarks



For info about presentation statistics for a frame, see <a href="https://msdn.microsoft.com/en-us/library/Bb173060(v=VS.85).aspx">DXGI_FRAME_STATISTICS</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174569(v=VS.85).aspx">IDXGISwapChain</a>
 

 

