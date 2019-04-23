---
UID: NF:d3d10.ID3D10Device.CheckFormatSupport
title: ID3D10Device::CheckFormatSupport (d3d10.h)
author: windows-sdk-content
description: Get the support of a given format on the installed video device.
old-location: direct3d10\id3d10device_checkformatsupport.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10device_checkformatsupport.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CheckFormatSupport, CheckFormatSupport method [Direct3D 10], CheckFormatSupport method [Direct3D 10],ID3D10Device interface, ID3D10Device interface [Direct3D 10],CheckFormatSupport method, ID3D10Device.CheckFormatSupport, ID3D10Device::CheckFormatSupport, d3d10/ID3D10Device::CheckFormatSupport, direct3d10.id3d10device_checkformatsupport, eaf02733-648b-44c6-4ca7-57aa2cecf913
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
 - ID3D10Device.CheckFormatSupport
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10Device::CheckFormatSupport


## -description


Get the support of a given format on the installed video device.


## -parameters




### -param Format [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a></b>

A <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a> enumeration that describes a format for which to check for support.


### -param pFormatSupport [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

A bitfield of <a href="https://msdn.microsoft.com/en-us/library/Bb205063(v=VS.85).aspx">D3D10_FORMAT_SUPPORT</a> enumeration values describing how the specified format is supported on the installed device. 
        The values are ORed together.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns S_OK if successful; otherwise, returns E_INVALIDARG if the <i>Format</i> parameter is <b>NULL</b>, or returns E_FAIL if the described 
      format does not exist.




## -remarks



Most format support is based on the Direct3D feature level. Only a few specific use cases require checking for support. 
      See <a href="https://docs.microsoft.com/en-us/windows/desktop/direct3ddxgi/format-support-for-direct3d-feature-level-10-0-hardware">Hardware Support for Direct3D 10 Formats</a> 
      and <a href="https://docs.microsoft.com/en-us/windows/desktop/direct3ddxgi/format-support-for-direct3d-feature-level-10-1-hardware">Hardware Support for Direct3D 10.1 Formats</a> for additional information.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173528(v=VS.85).aspx">ID3D10Device Interface</a>
 

 

