---
UID: NF:d3dcompiler.D3DSetBlobPart
title: D3DSetBlobPart function (d3dcompiler.h)
author: windows-sdk-content
description: Sets information in a compilation result.
old-location: direct3dhlsl\d3dsetblobpart.htm
tech.root: direct3dhlsl
ms.assetid: 244B094D-408A-4EC3-BC56-A7EE41D695E4
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: D3DSetBlobPart, D3DSetBlobPart function [HLSL], d3dcompiler/D3DSetBlobPart, direct3dhlsl.d3dsetblobpart
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
req.lib: D3DCompiler.lib
req.dll: D3DCompiler_47.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - D3DCompiler_47.dll
api_name:
 - D3DSetBlobPart
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# D3DSetBlobPart function


## -description


Sets information in a compilation result.


## -parameters




### -param pSrcData [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCVOID</a></b>

A pointer to compiled shader data.


### -param SrcDataSize [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">SIZE_T</a></b>

The length of the compiled shader data that <i>pSrcData</i> points to.


### -param Part [in]

Type: <b><a href="https://msdn.microsoft.com/333bc68a-0412-48e7-ac28-69ec5eea9ce8">D3D_BLOB_PART</a></b>

A <a href="https://msdn.microsoft.com/333bc68a-0412-48e7-ac28-69ec5eea9ce8">D3D_BLOB_PART</a>-typed value that specifies the part to set. Currently, you can update only private data; that is, <b>D3DSetBlobPart</b> currently only supports the <a href="https://msdn.microsoft.com/en-us/library/Ff728720(v=VS.85).aspx">D3D_BLOB_PRIVATE_DATA</a> value.


### -param Flags [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Flags that indicate how to set the blob part. Currently, no flags are defined; therefore, set to zero.


### -param pPart [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCVOID</a></b>

A pointer to data to set in the compilation result.


### -param PartSize [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">SIZE_T</a></b>

The length of the data that <i>pPart</i> points to.


### -param ppNewShader [out]

Type: <b><a href="https://msdn.microsoft.com/f6a04778-1ab9-4935-98b8-f814c6b4ebac">ID3DBlob</a>**</b>

A pointer to a buffer that receives the <a href="https://msdn.microsoft.com/f6a04778-1ab9-4935-98b8-f814c6b4ebac">ID3DBlob</a> interface for the new shader in which the new part data is set.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns one of the <a href="https://msdn.microsoft.com/c0856a58-b760-44e5-8acf-145720b403d1">Direct3D 11 return codes</a>.




## -remarks



<b>D3DSetBlobPart</b> modifies data in a compiled shader.  Currently, <b>D3DSetBlobPart</b> can update only the private data in a compiled shader. You can use  <b>D3DSetBlobPart</b> to attach arbitrary uninterpreted data to a compiled shader.

<div class="alert"><b>Note</b>  The D3dcompiler_44.dll or later version of the file contains the <b>D3DSetBlobPart</b> compiler function.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd607342(v=VS.85).aspx">Functions</a>
 

 

