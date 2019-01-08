---
UID: NF:dxgi1_4.IDXGISwapChain3.ResizeBuffers1
title: IDXGISwapChain3::ResizeBuffers1
author: windows-sdk-content
description: Changes the swap chain's back buffer size, format, and number of buffers, where the swap chain was created using a D3D12 command queue as an input device. This should be called when the application window is resized.
old-location: direct3ddxgi\idxgiswapchain3_resizebuffers1.htm
tech.root: direct3ddxgi
ms.assetid: 80983033-A348-4B25-B17E-AE7EE189EA1A
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDXGISwapChain3 interface [DXGI],ResizeBuffers1 method, IDXGISwapChain3.ResizeBuffers1, IDXGISwapChain3::ResizeBuffers1, ResizeBuffers1, ResizeBuffers1 method [DXGI], ResizeBuffers1 method [DXGI],IDXGISwapChain3 interface, direct3ddxgi.idxgiswapchain3_resizebuffers1, dxgi1_4/IDXGISwapChain3::ResizeBuffers1
ms.topic: method
req.header: dxgi1_4.h
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
 - IDXGISwapChain3.ResizeBuffers1
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGISwapChain3::ResizeBuffers1


## -description


Changes the swap chain's back buffer size, format, and number of buffers, where the swap chain was created using a D3D12 command queue as an input device.
          This should be called when the application window is resized.
        


## -parameters




### -param BufferCount [in]

Type: <b>UINT</b>

The number of buffers in the swap chain (including all back and front buffers).
            This number can be different from the number of buffers with which you created the swap chain.
            This number can't be greater than <b>DXGI_MAX_SWAP_CHAIN_BUFFERS</b>.
            Set this number to zero to preserve the existing number of buffers in the swap chain.
            You can't specify less than two buffers for the flip presentation model.
          


### -param Width [in]

Type: <b>UINT</b>

The new width of the back buffer. 
            If you specify zero, DXGI will use the width of the client area of the target window. 
            You can't specify the width as zero if you called the <a href="https://msdn.microsoft.com/8AE13082-F8C3-422A-A111-4E91488BD1AF">IDXGIFactory2::CreateSwapChainForComposition</a> method to create the swap chain for a composition surface.
          


### -param Height [in]

Type: <b>UINT</b>

The new height of the back buffer. 
            If you specify zero, DXGI will use the height of the client area of the target window. 
            You can't specify the height as zero if you called the <a href="https://msdn.microsoft.com/8AE13082-F8C3-422A-A111-4E91488BD1AF">IDXGIFactory2::CreateSwapChainForComposition</a> method to create the swap chain for a composition surface.
          


### -param Format [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a></b>

A <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>-typed value for the new format of the back buffer. 
            Set this value to <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT_UNKNOWN</a> to preserve the existing format of the back buffer. 
            The flip presentation model supports a more restricted set of formats than the bit-block transfer (bitblt) model.
          


### -param SwapChainFlags [in]

Type: <b>UINT</b>

A combination of <a href="https://msdn.microsoft.com/en-us/library/Bb173076(v=VS.85).aspx">DXGI_SWAP_CHAIN_FLAG</a>-typed values that are combined by using a bitwise OR operation.
            The resulting value specifies options for swap-chain behavior.
          


### -param pCreationNodeMask [in]

Type: <b>const UINT*</b>

An array of UINTs, of total size <i>BufferCount</i>, where the value indicates which node the back buffer should be created on.
            Buffers created using <b>ResizeBuffers1</b> with a non-null <i>pCreationNodeMask</i> array are visible to all nodes.
          


### -param ppPresentQueue [in]

Type: <b>IUnknown*</b>

An array of command queues (<a href="https://msdn.microsoft.com/88A4E8BA-02B9-48A1-8E46-2D2560544539">ID3D12CommandQueue</a> instances), of total size <i>BufferCount</i>.
            Each queue provided must match the corresponding creation node mask specified in the <i>pCreationNodeMask</i> array.
            When <b>Present()</b> is called, in addition to rotating to the next buffer for the next frame, the swapchain will also rotate through these command queues.
            This allows the app to control which queue requires synchronization for a given present operation.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns S_OK if successful; an error code otherwise.
            For a list of error codes, see <a href="https://msdn.microsoft.com/en-us/library/Bb509553(v=VS.85).aspx">DXGI_ERROR</a>.
          




## -remarks



This method is only valid to call when the swapchain was created using a D3D12 command queue (<a href="https://msdn.microsoft.com/88A4E8BA-02B9-48A1-8E46-2D2560544539">ID3D12CommandQueue</a>) as an input device.
        

When a swapchain is created on a multi-GPU adapter, the backbuffers are all created on node 1 and only a single command queue is supported.
          <b>ResizeBuffers1</b> enables applications to create backbuffers on different nodes, allowing a different command queue to be used with each node.
          These capabilities enable Alternate Frame Rendering (AFR) techniques to be used with the swapchain.
          See <a href="/windows/desktop/direct3d12/mulit-engine">Direct3D 12 Multi-Adapters</a>.
        

The only difference between <a href="https://msdn.microsoft.com/en-us/library/Bb174577(v=VS.85).aspx">IDXGISwapChain::ResizeBuffers</a> in Windows 8 versus Windows 7 is with
          flip presentation model swap chains that you create with the <a href="https://msdn.microsoft.com/en-us/library/Bb173077(v=VS.85).aspx">DXGI_SWAP_EFFECT_FLIP_SEQUENTIAL</a> or DXGI_SWAP_EFFECT_FLIP_DISCARD value set.
          In Windows 8, you must call <b>ResizeBuffers</b> to realize a transition between full-screen mode and windowed mode;
          otherwise, your next call to the <a href="https://msdn.microsoft.com/en-us/library/Bb174576(v=VS.85).aspx">IDXGISwapChain::Present</a> method fails.
        

Also see the Remarks section in <a href="https://msdn.microsoft.com/en-us/library/Bb174577(v=VS.85).aspx">IDXGISwapChain::ResizeBuffers</a>, all of which is relevant to <b>ResizeBuffers1</b>.
        




## -see-also




<a href="https://msdn.microsoft.com/3B91A70D-C635-46DF-871D-F1796D4E50E7">IDXGISwapChain3</a>
 

 

