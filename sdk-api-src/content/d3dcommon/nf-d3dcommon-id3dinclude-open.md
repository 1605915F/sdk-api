---
UID: NF:d3dcommon.ID3DInclude.Open
title: ID3DInclude::Open
author: windows-sdk-content
description: A user-implemented method for opening and reading the contents of a shader #include file.
old-location: direct3d11\id3dinclude_open.htm
tech.root: direct3d11
ms.assetid: 4d10c986-1cba-427c-ae90-f81b83be1b8b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3DInclude interface [Direct3D 11],Open method, ID3DInclude.Open, ID3DInclude::Open, Open, Open method [Direct3D 11], Open method [Direct3D 11],ID3DInclude interface, d3dcommon/ID3DInclude::Open, direct3d11.id3dinclude_open
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3dcommon.h
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
 - ID3DInclude.Open
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3DInclude::Open


## -description


A user-implemented method for opening and reading the contents of a shader #include file.


## -parameters




### -param IncludeType

Type: <b><a href="https://msdn.microsoft.com/98f0b0dd-9ff8-4321-a9ea-2deabc9529f2">D3D_INCLUDE_TYPE</a></b>

A <a href="https://msdn.microsoft.com/98f0b0dd-9ff8-4321-a9ea-2deabc9529f2">D3D_INCLUDE_TYPE</a>-typed value that indicates the location of the #include file.
          


### -param pFileName

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCSTR</a></b>

Name of the #include file.


### -param pParentData

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCVOID</a></b>

Pointer to the container that includes the #include file. The compiler might pass NULL in <i>pParentData</i>. For more information, see the "Searching for Include Files" section in <a href="https://msdn.microsoft.com/7624d55e-6466-4156-8f31-30f0d25a2883">Compile an Effect (Direct3D 11)</a>.
          


### -param ppData

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCVOID</a>*</b>

Pointer to the buffer  that contains the include directives. This pointer remains valid until you call<a href="https://msdn.microsoft.com/d4513e15-dfe7-4919-a278-d386f25e65e5">ID3DInclude::Close</a>.
          


### -param pBytes

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

Pointer to the number of bytes that <b>Open</b> returns in <i>ppData</i>.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

The user-implemented method must return S_OK. If <b>Open</b> fails when it reads the #include file, the application programming interface (API) that caused <b>Open</b> to be called fails. This failure can occur in one of the following situations:
              

<ul>
<li>The high-level shader language (HLSL) shader fails one of the <b>D3D10CompileShader***</b> functions.
              </li>
<li>The effect fails one of the <b>D3D10CreateEffect***</b> functions.
              </li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/2020ce65-3a6e-4a9f-9e97-b94e3c75f4f5">ID3DInclude</a>



<a href="https://msdn.microsoft.com/d4513e15-dfe7-4919-a278-d386f25e65e5">ID3DInclude::Close</a>
 

 

