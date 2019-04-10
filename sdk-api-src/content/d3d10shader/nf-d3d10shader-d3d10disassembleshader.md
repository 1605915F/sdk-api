---
UID: NF:d3d10shader.D3D10DisassembleShader
title: D3D10DisassembleShader function (d3d10shader.h)
author: windows-sdk-content
description: This function -- which disassembles a compiled shader into a text string that contains assembly instructions and register assignments -- has been deprecated. Instead, use D3DDisassemble.
old-location: direct3d10\d3d10disassembleshader.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\d3d10disassembleshader.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 3e4c4f2f-1754-2bbc-636d-9cea485ffad1, D3D10DisassembleShader, D3D10DisassembleShader function [Direct3D 10], d3d10shader/D3D10DisassembleShader, direct3d10.d3d10disassembleshader
ms.topic: function
req.header: d3d10shader.h
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
req.dll: D3D10.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - D3D10.dll
api_name:
 - D3D10DisassembleShader
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# D3D10DisassembleShader function


## -description


This function -- which disassembles a compiled shader into a text string that contains assembly instructions and register assignments -- has been deprecated. Instead, use <a href="https://msdn.microsoft.com/en-us/library/Dd607326(v=VS.85).aspx">D3DDisassemble</a>.


## -parameters




### -param pShader [in]

Type: <b>const void*</b>

A pointer to the compiled shader.


### -param BytecodeLength [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">SIZE_T</a></b>

The size of pShader.


### -param EnableColorCode [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

Include HTML tags in the output to color code the result.


### -param pComments [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCSTR</a></b>

The comment string at the top of the shader that identifies the shader constants and variables.


### -param ppDisassembly [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn933260(v=VS.85).aspx">ID3D10Blob</a>**</b>

Address of a buffer which contains the disassembled shader.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Return value




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb205157(v=VS.85).aspx">Shader Functions</a>
 

 

