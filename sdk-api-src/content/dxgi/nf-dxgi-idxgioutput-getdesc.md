---
UID: NF:dxgi.IDXGIOutput.GetDesc
title: IDXGIOutput::GetDesc
author: windows-sdk-content
description: Get a description of the output.
old-location: direct3ddxgi\idxgioutput_getdesc.htm
tech.root: direct3ddxgi
ms.assetid: VS|directx_sdk|~\idxgioutput_getdesc.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 895d1ca4-22a2-332a-34a7-b0c55200b423, GetDesc, GetDesc method [DXGI], GetDesc method [DXGI],IDXGIOutput interface, IDXGIOutput interface [DXGI],GetDesc method, IDXGIOutput.GetDesc, IDXGIOutput::GetDesc, direct3ddxgi.idxgioutput_getdesc, dxgi/IDXGIOutput::GetDesc
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
 - IDXGIOutput.GetDesc
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIOutput::GetDesc


## -description


Get a description of the output.


## -parameters




### -param pDesc [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173068(v=VS.85).aspx">DXGI_OUTPUT_DESC</a>*</b>

A pointer to the output description (see <a href="https://msdn.microsoft.com/en-us/library/Bb173068(v=VS.85).aspx">DXGI_OUTPUT_DESC</a>).


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns a code that indicates success or failure. S_OK if successful, <a href="https://msdn.microsoft.com/en-us/library/Bb509553(v=VS.85).aspx">DXGI_ERROR_INVALID_CALL</a> if <i>pDesc</i> is passed in as <b>NULL</b>.




## -remarks



 On a high DPI desktop, <b>GetDesc</b> returns the visualized screen size unless the app is marked high DPI aware. For info about writing DPI-aware Win32 apps, see <a href="https://msdn.microsoft.com/en-us/library/Mt843498(v=VS.85).aspx">High DPI</a>.




## -see-also




<a href="https://msdn.microsoft.com/b561b26b-961c-4d5e-8483-56b51b989bf7">DXGI Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174546(v=VS.85).aspx">IDXGIOutput</a>
 

 

