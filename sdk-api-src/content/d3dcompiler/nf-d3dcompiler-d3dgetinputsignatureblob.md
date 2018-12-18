---
UID: NF:d3dcompiler.D3DGetInputSignatureBlob
title: D3DGetInputSignatureBlob function
author: windows-sdk-content
description: Note  D3DGetInputSignatureBlob may be altered or unavailable for releases after Windows 8.1. Instead use D3DGetBlobPart with the D3D_BLOB_INPUT_SIGNATURE_BLOB value.  Gets the input signature from a compilation result.
old-location: direct3dhlsl\d3dgetinputsignatureblob.htm
tech.root: direct3dhlsl
ms.assetid: VS|directx_sdk|~\d3dgetinputsignatureblob.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 4f2b8180-4af5-06c2-bd88-b229e19ce686, D3DGetInputSignatureBlob, D3DGetInputSignatureBlob function [HLSL], d3dcompiler/D3DGetInputSignatureBlob, direct3dhlsl.d3dgetinputsignatureblob
ms.topic: function
req.header: d3dcompiler.h
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
req.lib: D3dcompiler_47.lib
req.dll: D3dcompiler_47.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - d3dcompiler_47.dll
api_name:
 - D3DGetInputSignatureBlob
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# D3DGetInputSignatureBlob function


## -description


<div class="alert"><b>Note</b>  <b>D3DGetInputSignatureBlob</b> may be altered or unavailable for releases after Windows 8.1. Instead use <a href="https://msdn.microsoft.com/cf9cea53-e7a3-4473-bfdf-0cdeb8370974">D3DGetBlobPart</a> with the <a href="https://msdn.microsoft.com/en-us/library/Ff728720(v=VS.85).aspx">D3D_BLOB_INPUT_SIGNATURE_BLOB</a> value. </div><div> </div>Gets the input signature from a compilation result.


## -parameters




### -param pSrcData [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCVOID</a></b>

A pointer to source data as compiled HLSL code.


### -param SrcDataSize [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">SIZE_T</a></b>

Length of <i>pSrcData</i>.


### -param ppSignatureBlob [out]

Type: <b><a href="https://msdn.microsoft.com/f6a04778-1ab9-4935-98b8-f814c6b4ebac">ID3DBlob</a>**</b>

A pointer to a buffer that receives the <a href="https://msdn.microsoft.com/f6a04778-1ab9-4935-98b8-f814c6b4ebac">ID3DBlob</a> interface that contains a compiled shader.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns one of the <a href="https://msdn.microsoft.com/c0856a58-b760-44e5-8acf-145720b403d1">Direct3D 11 return codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd607342(v=VS.85).aspx">Functions</a>
 

 

