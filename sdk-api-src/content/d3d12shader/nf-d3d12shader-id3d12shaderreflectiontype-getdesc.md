---
UID: NF:d3d12shader.ID3D12ShaderReflectionType.GetDesc
title: ID3D12ShaderReflectionType::GetDesc
author: windows-sdk-content
description: Gets the description of a shader-reflection-variable type.
old-location: direct3d12\id3d12shaderreflectiontype_getdesc.htm
tech.root: direct3d12
ms.assetid: E5C28FFE-5BA4-436F-9CDB-215B5B9918F9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDesc, GetDesc method, GetDesc method,ID3D12ShaderReflectionType interface, ID3D12ShaderReflectionType interface,GetDesc method, ID3D12ShaderReflectionType.GetDesc, ID3D12ShaderReflectionType::GetDesc, d3d12shader/ID3D12ShaderReflectionType::GetDesc, direct3d12.id3d12shaderreflectiontype_getdesc
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
 - ID3D12ShaderReflectionType.GetDesc
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12ShaderReflectionType::GetDesc


## -description


Gets the description of a shader-reflection-variable type.
        


## -parameters




### -param pDesc [out]

Type: <b><a href="https://msdn.microsoft.com/B0AF7987-B25B-4496-9B8F-1D9C16DF5E50">D3D12_SHADER_TYPE_DESC</a>*</b>

A pointer to a shader-type description (see <a href="https://msdn.microsoft.com/B0AF7987-B25B-4496-9B8F-1D9C16DF5E50">D3D12_SHADER_TYPE_DESC</a>).
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns one of the <a href="https://msdn.microsoft.com/5F6CC962-7DB7-489F-82A4-9388313014D3">Direct3D 12 Return Codes</a>.
          




## -remarks



This method's interface is hosted in the out-of-box DLL D3DCompiler_xx.dll.
      




## -see-also




<a href="https://msdn.microsoft.com/78FF30C5-7F23-489D-9E9D-916F6CE09C0E">ID3D12ShaderReflectionType</a>
 

 

