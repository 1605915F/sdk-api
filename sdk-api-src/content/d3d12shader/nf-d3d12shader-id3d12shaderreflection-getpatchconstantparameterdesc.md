---
UID: NF:d3d12shader.ID3D12ShaderReflection.GetPatchConstantParameterDesc
title: ID3D12ShaderReflection::GetPatchConstantParameterDesc (d3d12shader.h)
author: windows-sdk-content
description: Gets a patch-constant parameter description for a shader.
old-location: direct3d12\id3d12shaderreflection_getpatchconstantparameterdesc.htm
tech.root: direct3d12
ms.assetid: 01353250-0C8F-4C72-93CE-64BEF52EB985
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPatchConstantParameterDesc, GetPatchConstantParameterDesc method, GetPatchConstantParameterDesc method,ID3D12ShaderReflection interface, ID3D12ShaderReflection interface,GetPatchConstantParameterDesc method, ID3D12ShaderReflection.GetPatchConstantParameterDesc, ID3D12ShaderReflection::GetPatchConstantParameterDesc, d3d12shader/ID3D12ShaderReflection::GetPatchConstantParameterDesc, direct3d12.id3d12shaderreflection_getpatchconstantparameterdesc
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
 - ID3D12ShaderReflection.GetPatchConstantParameterDesc
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12ShaderReflection::GetPatchConstantParameterDesc


## -description


Gets a patch-constant parameter description for a shader.
        


## -parameters




### -param ParameterIndex [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

A zero-based parameter index.
          


### -param pDesc [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn960205(v=VS.85).aspx">D3D12_SIGNATURE_PARAMETER_DESC</a>*</b>

A pointer to a shader-input-signature description. See <a href="https://msdn.microsoft.com/en-us/library/Dn960205(v=VS.85).aspx">D3D12_SIGNATURE_PARAMETER_DESC</a>.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns one of the <a href="https://msdn.microsoft.com/5F6CC962-7DB7-489F-82A4-9388313014D3">Direct3D 12 Return Codes</a>.
          




## -remarks



This method's interface is hosted in the out-of-box DLL D3DCompiler_xx.dll.
      




## -see-also




<a href="https://msdn.microsoft.com/145F2CCB-C076-42BE-8AF4-74349CDF6B02">ID3D12ShaderReflection</a>
 

 

