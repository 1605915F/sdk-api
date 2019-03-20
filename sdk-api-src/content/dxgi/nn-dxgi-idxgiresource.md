---
UID: NN:dxgi.IDXGIResource
title: IDXGIResource (dxgi.h)
author: windows-sdk-content
description: An IDXGIResource interface allows resource sharing and identifies the memory that a resource resides in.
old-location: direct3ddxgi\idxgiresource.htm
tech.root: direct3ddxgi
ms.assetid: VS|directx_sdk|~\idxgiresource.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 74b46980-220f-d8c0-f488-2656b735bb5d, IDXGIResource, IDXGIResource interface [DXGI], IDXGIResource interface [DXGI],described, direct3ddxgi.idxgiresource, dxgi/IDXGIResource
ms.topic: interface
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
 - IDXGIResource
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIResource interface


## -description


An <b>IDXGIResource</b> interface allows resource sharing and identifies the memory that a resource resides in.
      


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDXGIResource</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Bb174528(v=VS.85).aspx">IDXGIDeviceSubObject</a>. <b>IDXGIResource</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDXGIResource</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb174561(v=VS.85).aspx">GetEvictionPriority</a>
</td>
<td align="left" width="63%">
Get the eviction priority.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb174562(v=VS.85).aspx">GetSharedHandle</a>
</td>
<td align="left" width="63%">
Gets the handle to a shared resource.

<div class="alert"><b>Note</b>  Starting with Direct3D 11.1, we recommend not to use <a href="https://msdn.microsoft.com/en-us/library/Bb174562(v=VS.85).aspx">GetSharedHandle</a> anymore to retrieve the handle to a shared resource. Instead, use <a href="https://msdn.microsoft.com/7A53616A-E7AB-4EB7-9B8F-ED43A70B691C">IDXGIResource1::CreateSharedHandle</a> to get a handle for sharing. To use <b>IDXGIResource1::CreateSharedHandle</b>, you  must create the resource as shared and specify that it uses NT handles (that is, you set the <a href="https://msdn.microsoft.com/2a324055-21b0-4dad-a8e0-781905329dc2">D3D11_RESOURCE_MISC_SHARED_NTHANDLE</a> flag). We also recommend that you create shared resources that use NT handles so you can use <a href="https://msdn.microsoft.com/9b84891d-62ca-4ddc-97b7-c4c79482abd9">CloseHandle</a>, <a href="https://msdn.microsoft.com/9c8da574-5bda-49f1-a6b6-c026639d6504">DuplicateHandle</a>, and so on on those shared resources.</div>
<div> </div>
</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb174563(v=VS.85).aspx">GetUsage</a>
</td>
<td align="left" width="63%">
Get the expected resource usage.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb174564(v=VS.85).aspx">SetEvictionPriority</a>
</td>
<td align="left" width="63%">
Set the priority for evicting the resource from memory.

</td>
</tr>
</table> 


## -remarks



To find out what type of memory a resource is currently located in, use <a href="https://msdn.microsoft.com/en-us/library/Bb174533(v=VS.85).aspx">IDXGIDevice::QueryResourceResidency</a>. To share resources between processes, use <a href="https://msdn.microsoft.com/en-us/library/Bb173598(v=VS.85).aspx">ID3D10Device::OpenSharedResource</a>. For information about how to share resources between multiple Windows graphics APIs, including Direct3D 11, Direct2D, Direct3D 10, and Direct3D 9Ex, see <a href="https://msdn.microsoft.com/65abf33e-3d15-42ff-99bd-674f24da773e">Surface Sharing Between Windows Graphics APIs</a>.
          

You can retrieve the <b>IDXGIResource</b>  interface from any video memory resource that you create from a Direct3D 10 and later function. Any Direct3D object that supports <a href="https://msdn.microsoft.com/en-us/library/Bb173829(v=VS.85).aspx">ID3D10Resource</a> or <a href="https://msdn.microsoft.com/3823ec00-cb3c-43ce-9f1a-be4e1e99d587">ID3D11Resource</a> also supports <b>IDXGIResource</b>. For example, the Direct3D 2D texture object that you create from <a href="https://msdn.microsoft.com/69950ce7-9c8e-4f00-860d-e118e2bbc81a">ID3D11Device::CreateTexture2D</a> supports <b>IDXGIResource</b>. You can call <a href="https://msdn.microsoft.com/54d5ff80-18db-43f2-b636-f93ac053146d">QueryInterface</a> on the 2D texture object (<a href="https://msdn.microsoft.com/49cd6e21-6cb1-45ea-b83a-3c93f0560915">ID3D11Texture2D</a>) to retrieve the <b>IDXGIResource</b> interface. For example, to retrieve the <b>IDXGIResource</b>  interface from  the 2D texture object, use the following code.
          


```
IDXGIResource * pDXGIResource;
hr = g_pd3dTexture2D->QueryInterface(__uuidof(IDXGIResource), (void **)&pDXGIResource);
```


<b>Windows Phone 8:
        </b> This API is supported.
      




## -see-also




<a href="https://msdn.microsoft.com/b561b26b-961c-4d5e-8483-56b51b989bf7">DXGI Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174528(v=VS.85).aspx">IDXGIDeviceSubObject</a>
 

 

