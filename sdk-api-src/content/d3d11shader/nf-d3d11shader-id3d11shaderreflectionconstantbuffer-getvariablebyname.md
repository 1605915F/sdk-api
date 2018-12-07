---
UID: NF:d3d11shader.ID3D11ShaderReflectionConstantBuffer.GetVariableByName
title: ID3D11ShaderReflectionConstantBuffer::GetVariableByName
author: windows-sdk-content
description: Get a shader-reflection variable by name.
old-location: direct3d11\id3d11shaderreflectionconstantbuffer_getvariablebyname.htm
tech.root: direct3d11
ms.assetid: daa14557-0987-4498-a2f5-428497805eca
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 613cfca7-07e9-dcae-c494-e5cdf1002b8c, GetVariableByName, GetVariableByName method [Direct3D 11], GetVariableByName method [Direct3D 11],ID3D11ShaderReflectionConstantBuffer interface, ID3D11ShaderReflectionConstantBuffer interface [Direct3D 11],GetVariableByName method, ID3D11ShaderReflectionConstantBuffer.GetVariableByName, ID3D11ShaderReflectionConstantBuffer::GetVariableByName, d3d11shader/ID3D11ShaderReflectionConstantBuffer::GetVariableByName, direct3d11.id3d11shaderreflectionconstantbuffer_getvariablebyname
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d11shader.h
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
req.lib: D3DCompiler.lib
req.dll: D3DCompiler_47.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3DCompiler_47.dll
api_name:
 - ID3D11ShaderReflectionConstantBuffer.GetVariableByName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11ShaderReflectionConstantBuffer::GetVariableByName


## -description


Get a shader-reflection variable by name.


## -parameters




### -param Name [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">LPCSTR</a></b>

Variable name.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Ff476607(v=VS.85).aspx">ID3D11ShaderReflectionVariable</a>*</b>

Returns a sentinel object (end of list marker). To determine if GetVariableByName successfully completed, call <a href="https://msdn.microsoft.com/en-us/library/Ff476608(v=VS.85).aspx">ID3D11ShaderReflectionVariable::GetDesc</a> and check the returned <b>HRESULT</b>; any return value other than success means that GetVariableByName failed.




## -remarks



This method's interface is hosted in the out-of-box DLL D3DCompiler_xx.dll.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff476591(v=VS.85).aspx">ID3D11ShaderReflectionConstantBuffer Interface</a>
 

 

