---
UID: NF:dxgi1_4.IDXGISwapChain3.CheckColorSpaceSupport
title: IDXGISwapChain3::CheckColorSpaceSupport
author: windows-sdk-content
description: Checks the swap chain's support for color space.
old-location: direct3ddxgi\idxgiswapchain3_checkcolorspacesupport.htm
tech.root: direct3ddxgi
ms.assetid: 87AFB541-EC10-45E6-97CC-1B48084D00EE
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CheckColorSpaceSupport, CheckColorSpaceSupport method [DXGI], CheckColorSpaceSupport method [DXGI],IDXGISwapChain3 interface, IDXGISwapChain3 interface [DXGI],CheckColorSpaceSupport method, IDXGISwapChain3.CheckColorSpaceSupport, IDXGISwapChain3::CheckColorSpaceSupport, direct3ddxgi.idxgiswapchain3_checkcolorspacesupport, dxgi1_4/IDXGISwapChain3::CheckColorSpaceSupport
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dxgi1_4.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dxgi.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dxgi.lib
 - Dxgi.dll
api_name:
 - IDXGISwapChain3.CheckColorSpaceSupport
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGISwapChain3::CheckColorSpaceSupport


## -description


Checks the swap chain's support for color space.


## -parameters




### -param ColorSpace [in]

Type: <b><a href="https://msdn.microsoft.com/E25C933F-0DB3-4BC4-9755-9361B2B9B9CB">DXGI_COLOR_SPACE_TYPE</a></b>

A <a href="https://msdn.microsoft.com/E25C933F-0DB3-4BC4-9755-9361B2B9B9CB">DXGI_COLOR_SPACE_TYPE</a>-typed value that specifies color space type to check support for.


### -param pColorSpaceSupport [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

A pointer to a variable that receives a combination of <a href="https://msdn.microsoft.com/D0479BB0-C433-49C3-9D63-5E99EC4565A9">DXGI_SWAP_CHAIN_COLOR_SPACE_SUPPORT_FLAG</a>-typed values that are combined by using a bitwise OR operation. The resulting value specifies options for color space support. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns <b>S_OK</b> on success, or it returns one of the error codes that are described in the <a href="https://msdn.microsoft.com/en-us/library/Bb509553(v=VS.85).aspx">DXGI_ERROR</a> topic.




## -see-also




<a href="https://msdn.microsoft.com/3B91A70D-C635-46DF-871D-F1796D4E50E7">IDXGISwapChain3</a>
 

 

