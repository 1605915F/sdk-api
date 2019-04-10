---
UID: NN:dxgi.IDXGIDevice1
title: IDXGIDevice1 (dxgi.h)
author: windows-sdk-content
description: An IDXGIDevice1 interface implements a derived class for DXGI objects that produce image data.
old-location: direct3ddxgi\idxgidevice1.htm
tech.root: direct3ddxgi
ms.assetid: a0ba0fa3-489a-4eff-9e49-b231ab472ee4
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 9db12484-8e98-1317-79e4-cbaa511683b8, IDXGIDevice1, IDXGIDevice1 interface [DXGI], IDXGIDevice1 interface [DXGI],described, direct3ddxgi.idxgidevice1, dxgi/IDXGIDevice1
ms.topic: interface
req.header: dxgi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - IDXGIDevice1
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIDevice1 interface


## -description


An <b>IDXGIDevice1</b> interface implements a derived class for DXGI objects that produce image data.
      


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDXGIDevice1</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Bb174527(v=VS.85).aspx">IDXGIDevice</a>. <b>IDXGIDevice1</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDXGIDevice1</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/87b98c47-3556-4588-97b2-c935d7052286">GetMaximumFrameLatency</a>
</td>
<td align="left" width="63%">
Gets the number of frames that the system is allowed to queue for rendering.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ea477f33-2dba-44ac-9b47-8fd2ce6cec30">SetMaximumFrameLatency</a>
</td>
<td align="left" width="63%">
Sets the number of frames that the system is allowed to queue for rendering.

</td>
</tr>
</table> 


## -remarks



This interface is not supported by Direct3D 12 devices. Direct3D 12 applications have direct control over their swapchain management, so better latency control should be handled by the application. You can make use of Waitable objects (refer to <a href="https://msdn.microsoft.com/en-us/library/Bb173076(v=VS.85).aspx">DXGI_SWAP_CHAIN_FLAG_FRAME_LATENCY_WAITABLE_OBJECT</a>) and the <a href="https://msdn.microsoft.com/AF3F03F2-38B4-474A-8A66-86A93D776EA0">IDXGISwapChain2::SetMaximumFrameLatency</a> method if desired.



This interface is not supported by DXGI 1.0, which shipped in Windows Vista and Windows Server 2008. DXGI 1.1 support is required, which is available on
          Windows 7, Windows Server 2008 R2, and as an update to Windows Vista with Service Pack 2 (SP2) (<a href="http://go.microsoft.com/fwlink/p/?linkid=160189">KB 971644</a>) and Windows Server 2008 (<a href="http://go.microsoft.com/fwlink/p/?linkid=183689">KB 971512</a>).
        

The <b>IDXGIDevice1</b> interface is designed for use by DXGI objects that need access to other DXGI objects. This interface is useful to
          applications that do not use Direct3D to communicate with DXGI.
        

The Direct3D create device functions return a Direct3D device object. This Direct3D device object implements the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. You can query this Direct3D device object for the device's
          corresponding <b>IDXGIDevice1</b> interface. To retrieve the <b>IDXGIDevice1</b>  interface of a Direct3D device, use the following code:
        


```
IDXGIDevice1 * pDXGIDevice;
hr = g_pd3dDevice->QueryInterface(__uuidof(IDXGIDevice1), (void **)&pDXGIDevice);

```


<b>Windows Phone 8:
        </b> This API is supported.
      




## -see-also




<a href="https://msdn.microsoft.com/b561b26b-961c-4d5e-8483-56b51b989bf7">DXGI Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174527(v=VS.85).aspx">IDXGIDevice</a>
 

 

