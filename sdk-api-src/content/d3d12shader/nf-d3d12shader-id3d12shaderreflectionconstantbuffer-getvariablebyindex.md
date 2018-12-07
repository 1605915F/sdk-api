---
UID: NF:d3d12shader.ID3D12ShaderReflectionConstantBuffer.GetVariableByIndex
title: ID3D12ShaderReflectionConstantBuffer::GetVariableByIndex
author: windows-sdk-content
description: Gets a shader-reflection variable by index.
old-location: direct3d12\id3d12shaderreflectionconstantbuffer_getvariablebyindex.htm
tech.root: direct3d12
ms.assetid: F7083A4D-ADD4-4C6F-A031-ABF16A3C351C
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetVariableByIndex, GetVariableByIndex method, GetVariableByIndex method,ID3D12ShaderReflectionConstantBuffer interface, ID3D12ShaderReflectionConstantBuffer interface,GetVariableByIndex method, ID3D12ShaderReflectionConstantBuffer.GetVariableByIndex, ID3D12ShaderReflectionConstantBuffer::GetVariableByIndex, d3d12shader/ID3D12ShaderReflectionConstantBuffer::GetVariableByIndex, direct3d12.id3d12shaderreflectionconstantbuffer_getvariablebyindex
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d12shader.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - d3d12shader.h
api_name:
 - ID3D12ShaderReflectionConstantBuffer.GetVariableByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12ShaderReflectionConstantBuffer::GetVariableByIndex


## -description


Gets a shader-reflection variable by index.
        


## -parameters




### -param Index [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

Zero-based index.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn933696(v=VS.85).aspx">ID3D12ShaderReflectionVariable</a>*</b>

A pointer to a shader-reflection variable interface (see <a href="https://msdn.microsoft.com/en-us/library/Dn933696(v=VS.85).aspx">ID3D12ShaderReflectionVariable Interface</a>).
          




## -remarks



This method's interface is hosted in the out-of-box DLL D3DCompiler_xx.dll.
      




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn933680(v=VS.85).aspx">ID3D12ShaderReflectionConstantBuffer</a>
 

 

