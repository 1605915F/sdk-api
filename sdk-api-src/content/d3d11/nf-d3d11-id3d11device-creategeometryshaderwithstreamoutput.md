---
UID: NF:d3d11.ID3D11Device.CreateGeometryShaderWithStreamOutput
title: ID3D11Device::CreateGeometryShaderWithStreamOutput (d3d11.h)
author: windows-sdk-content
description: Creates a geometry shader that can write to streaming output buffers.
old-location: direct3d11\id3d11device_creategeometryshaderwithstreamoutput.htm
tech.root: direct3d11
ms.assetid: 69499121-6f35-4cf1-b115-9ffdce26e4b0
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 39026c1a-ac13-562f-6f6e-86f1981ebb87, CreateGeometryShaderWithStreamOutput, CreateGeometryShaderWithStreamOutput method [Direct3D 11], CreateGeometryShaderWithStreamOutput method [Direct3D 11],ID3D11Device interface, ID3D11Device interface [Direct3D 11],CreateGeometryShaderWithStreamOutput method, ID3D11Device.CreateGeometryShaderWithStreamOutput, ID3D11Device::CreateGeometryShaderWithStreamOutput, d3d11/ID3D11Device::CreateGeometryShaderWithStreamOutput, direct3d11.id3d11device_creategeometryshaderwithstreamoutput
ms.topic: method
req.header: d3d11.h
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
req.lib: D3D11.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D11.lib
 - D3D11.dll
api_name:
 - ID3D11Device.CreateGeometryShaderWithStreamOutput
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11Device::CreateGeometryShaderWithStreamOutput


## -description


Creates a geometry shader that can write to streaming output buffers.


## -parameters




### -param pShaderBytecode [in]

Type: <b>const void*</b>

A pointer to the compiled geometry shader for a standard geometry shader plus stream output. For info on how to get this pointer, see <a href="https://msdn.microsoft.com/en-us/library/Bb509703(v=VS.85).aspx">Getting a Pointer to a Compiled Shader</a>.

To create the stream output without using a geometry shader, pass a pointer to the output signature for the prior stage. To obtain this output signature, call the <a href="https://msdn.microsoft.com/en-us/library/Dd607331(v=VS.85).aspx">D3DGetOutputSignatureBlob</a> compiler function. You can also pass a pointer to the compiled shader for the prior stage (for example, the <a href="https://msdn.microsoft.com/library/Bb205146(v=VS.85).aspx">vertex-shader stage</a> or <a href="https://msdn.microsoft.com/en-us/library/Ff476340(v=VS.85).aspx">domain-shader stage</a>). This compiled shader provides the output signature for the data.
            


### -param BytecodeLength [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">SIZE_T</a></b>

Size of the compiled geometry shader.


### -param pSODeclaration [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/c40e8db6-e26f-4c61-a812-f60eae43e86b">D3D11_SO_DECLARATION_ENTRY</a>*</b>

Pointer to a <a href="https://msdn.microsoft.com/c40e8db6-e26f-4c61-a812-f60eae43e86b">D3D11_SO_DECLARATION_ENTRY</a> array. Cannot be <b>NULL</b> if NumEntries &gt; 0.
          


### -param NumEntries [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of entries in the stream output declaration ( ranges from 0 to D3D11_SO_STREAM_COUNT * D3D11_SO_OUTPUT_COMPONENT_COUNT ).


### -param pBufferStrides [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

An array of buffer strides; each stride is the size of an element for that buffer.


### -param NumStrides [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of strides (or buffers) in <i>pBufferStrides</i> (ranges from 0 to D3D11_SO_BUFFER_SLOT_COUNT).
          


### -param RasterizedStream [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The index number of the stream to be sent to the rasterizer stage (ranges from 0 to D3D11_SO_STREAM_COUNT - 1).
              Set to D3D11_SO_NO_RASTERIZED_STREAM if no stream is to be rasterized.
            


### -param pClassLinkage [in, optional]

Type: <b><a href="https://msdn.microsoft.com/eac03911-d881-4304-9598-912321ac0b0c">ID3D11ClassLinkage</a>*</b>

A pointer to a class linkage interface (see <a href="https://msdn.microsoft.com/eac03911-d881-4304-9598-912321ac0b0c">ID3D11ClassLinkage</a>); the value can be <b>NULL</b>.
          


### -param ppGeometryShader [out, optional]

Type: <b><a href="https://msdn.microsoft.com/c2b5863d-5773-4719-b1d0-2026f55fcef3">ID3D11GeometryShader</a>**</b>

Address of a pointer to an <a href="https://msdn.microsoft.com/c2b5863d-5773-4719-b1d0-2026f55fcef3">ID3D11GeometryShader</a> interface, representing the geometry shader that was created.
            Set this to <b>NULL</b> to validate the other parameters; if validation passes, the method will return S_FALSE instead of S_OK.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the <a href="https://msdn.microsoft.com/c0856a58-b760-44e5-8acf-145720b403d1">Direct3D 11 Return Codes</a>.
          




## -remarks



For more info about using <b>CreateGeometryShaderWithStreamOutput</b>, see <a href="https://msdn.microsoft.com/en-us/library/Bb205122(v=VS.85).aspx">Create a Geometry-Shader Object with Stream Output</a>.
        

The Direct3D 11.1 runtime, which is available starting with Windows 8, provides the following new functionality for <b>CreateGeometryShaderWithStreamOutput</b>.
        

The following shader model 5.0 instructions are available to just pixel shaders and compute shaders in the Direct3D 11.0 runtime. For the Direct3D 11.1 runtime, because unordered access views (UAV) are available at all shader stages, you can use these instructions in all shader stages.

Therefore, if you use the following shader model 5.0 instructions in a geometry shader, you can successfully pass the compiled geometry shader to <i>pShaderBytecode</i>. That is, the call to <b>CreateGeometryShaderWithStreamOutput</b> succeeds.
        

If you pass a compiled shader to <i>pShaderBytecode</i> that uses any of the following instructions on a device that doesn’t support UAVs at every shader stage (including existing drivers that are not implemented to support UAVs at every shader stage), <b>CreateGeometryShaderWithStreamOutput</b> fails.  <b>CreateGeometryShaderWithStreamOutput</b> also fails if the shader tries to use a UAV slot beyond the set of UAV slots that the hardware supports.
        

<ul>
<li>
<a href="https://msdn.microsoft.com/F9F5583F-E3D0-447F-9227-BBB1B4E71934">dcl_uav_typed</a>
</li>
<li>
<a href="https://msdn.microsoft.com/D0F43FF8-FF1C-4E42-AF42-F528C98FD680">dcl_uav_raw</a>
</li>
<li>
<a href="https://msdn.microsoft.com/40D6B8F7-8A41-4EFE-A8A3-44A646B4D43B">dcl_uav_structured</a>
</li>
<li>
<a href="https://msdn.microsoft.com/F7DBA80D-4DD5-4271-B571-24FB6188ABFE">ld_raw</a>
</li>
<li>
<a href="https://msdn.microsoft.com/ED572B76-FF6C-405E-9110-4B12AD5E5AE6">ld_structured</a>
</li>
<li>
<a href="https://msdn.microsoft.com/E5E03311-3596-4497-9271-FE6445DBFC62">ld_uav_typed</a>
</li>
<li>
<a href="https://msdn.microsoft.com/D166116A-CF4E-4020-9F6A-F9CEEFCDAB21">store_raw</a>
</li>
<li>
<a href="https://msdn.microsoft.com/8080B2CA-5BDA-4F01-8B2B-B85BDD58C5AF">store_structured</a>
</li>
<li>
<a href="https://msdn.microsoft.com/AD8E035B-DACD-4241-A05B-7D6DC8E3222C">store_uav_typed</a>
</li>
<li>
<a href="https://msdn.microsoft.com/DCA637FE-8F5C-41D0-8B5E-F913463BA387">sync_uglobal</a>
</li>
<li>All atomics and immediate atomics (for example, <a href="https://msdn.microsoft.com/5FA731E0-7D18-4416-9579-FCA01FF5FC38">atomic_and</a> and <a href="https://msdn.microsoft.com/DA2A70C3-57BD-41F0-865C-235AA4DF1A52">imm_atomic_and</a>)
          </li>
</ul>
<b>Windows Phone 8:
        </b> This API is supported.
      




## -see-also




<a href="https://msdn.microsoft.com/2f2559d9-1cd6-44f6-90e2-ee0f86e39f78">ID3D11Device</a>
 

 

