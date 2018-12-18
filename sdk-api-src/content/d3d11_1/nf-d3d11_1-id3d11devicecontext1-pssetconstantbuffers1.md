---
UID: NF:d3d11_1.ID3D11DeviceContext1.PSSetConstantBuffers1
title: ID3D11DeviceContext1::PSSetConstantBuffers1
author: windows-sdk-content
description: Sets the constant buffers that the pixel shader pipeline stage uses, and enables the shader to access other parts of the buffer.
old-location: direct3d11\id3d11devicecontext1_pssetconstantbuffers1.htm
tech.root: direct3d11
ms.assetid: 4B05144B-7766-4AE6-9B9F-C439B4BF0220
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3D11DeviceContext1 interface [Direct3D 11],PSSetConstantBuffers1 method, ID3D11DeviceContext1.PSSetConstantBuffers1, ID3D11DeviceContext1::PSSetConstantBuffers1, PSSetConstantBuffers1, PSSetConstantBuffers1 method [Direct3D 11], PSSetConstantBuffers1 method [Direct3D 11],ID3D11DeviceContext1 interface, d3d11_1/ID3D11DeviceContext1::PSSetConstantBuffers1, direct3d11.id3d11devicecontext1_pssetconstantbuffers1
ms.topic: method
req.header: d3d11_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - ID3D11DeviceContext1.PSSetConstantBuffers1
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11DeviceContext1::PSSetConstantBuffers1


## -description


Sets the constant buffers that the pixel shader pipeline stage uses, and enables the shader to access other parts of the buffer.
      


## -parameters




### -param StartSlot [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index into the device's zero-based array to begin setting constant buffers to (ranges from 0 to D3D11_COMMONSHADER_CONSTANT_BUFFER_API_SLOT_COUNT - 1).
          


### -param NumBuffers [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Number of buffers to set (ranges from 0 to D3D11_COMMONSHADER_CONSTANT_BUFFER_API_SLOT_COUNT - <i>StartSlot</i>).
          


### -param ppConstantBuffers [in, optional]

Type: <b><a href="https://msdn.microsoft.com/7224de57-75cb-4d68-9d70-f5dd2f92b1fd">ID3D11Buffer</a>*</b>

Array of constant buffers being given to the device.
          


### -param pFirstConstant [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

An array that holds the offsets into the buffers that  <i>ppConstantBuffers</i> specifies.
            Each offset specifies where, from the shader's point of view, each constant buffer starts.
            Each offset is measured in shader constants, which are 16 bytes (4*32-bit components).
            Therefore, an offset of 16 indicates that the start of the associated constant buffer is 256 bytes into the constant buffer.
            Each offset must be a multiple of 16 constants.
          


### -param pNumConstants [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

An array that holds the numbers of constants in the buffers that  <i>ppConstantBuffers</i> specifies.
            Each number specifies the number of constants that are contained in the constant buffer that the shader uses.
            Each number of constants starts from its respective offset that is specified in the <i>pFirstConstant</i> array.
            Each number of constants must be a multiple of 16 constants, in the range [0..4096].
          


## -returns



Returns nothing.
          




## -remarks



To enable the shader to access other parts of the buffer, call
          <b>PSSetConstantBuffers1</b> instead of <a href="https://msdn.microsoft.com/03e5f255-3a5d-4c77-ad3b-5a188c9eb35b">PSSetConstantBuffers</a>.
          <b>PSSetConstantBuffers1</b> has additional parameters <i>pFirstConstant</i> and <i>pNumConstants</i>.
        

The runtime drops the call to <b>PSSetConstantBuffers1</b> if the numbers of constants to which <i>pNumConstants</i> points
          is larger than the maximum constant buffer size that is supported by shaders.
          The maximum constant buffer size that is supported by shaders holds 4096 constants, where each constant has four 32-bit components.
        

The values in the elements of the <i>pFirstConstant</i> and <i>pFirstConstant</i> + <i>pNumConstants</i> arrays can exceed the length of each buffer;
          from the shader's point of view, the constant buffer is the intersection of the actual memory allocation for the buffer and
          the following window (range):
        

[value in an element of <i>pFirstConstant</i>, value in an element of <i>pFirstConstant</i> + value in an element of <i>pNumConstants</i>]
        

That is, the window is the range is from (value in an element of <i>pFirstConstant</i>) to (value in an element of <i>pFirstConstant</i> + value in an element of <i>pNumConstants</i>).
        

The runtime also drops the call to <b>PSSetConstantBuffers1</b> on existing drivers that do not support this offsetting.
        

The runtime will emulate this feature for <a href="https://msdn.microsoft.com/en-us/library/Ff476876(v=VS.85).aspx">feature level</a> 9.1, 9.2, and 9.3; therefore, this feature is supported for feature level 9.1, 9.2, and 9.3.
          This feature is always available on new drivers for feature level 10 and higher.
        

From the shader’s point of view, element [0] in the constant buffers array is the constant at <i>pFirstConstant</i>.
        

Out of bounds access to the constant buffers from the shader to the range that is defined by <i>pFirstConstant</i> and <i>pNumConstants</i> returns 0.
        

If <i>pFirstConstant</i> and <i>pNumConstants</i> arrays are <b>NULL</b>, you get the same result as if you were binding the entire buffer into view.
          You get this same result if you call the <a href="https://msdn.microsoft.com/03e5f255-3a5d-4c77-ad3b-5a188c9eb35b">PSSetConstantBuffers</a> method.
          If the buffer is larger than the maximum constant buffer size that is supported by shaders (4096 elements), the shader can access only the first 4096 constants.
        

If either <i>pFirstConstant</i> or <i>pNumConstants</i> is <b>NULL</b>, the other parameter must also be <b>NULL</b>.
        

<h3><a id="Calling_PSSetConstantBuffers1_with_command_list_emulation"></a><a id="calling_pssetconstantbuffers1_with_command_list_emulation"></a><a id="CALLING_PSSETCONSTANTBUFFERS1_WITH_COMMAND_LIST_EMULATION"></a>Calling PSSetConstantBuffers1 with command list emulation</h3>
The runtime's <a href="https://msdn.microsoft.com/4f581bc7-6c5e-4e56-b768-7f3cc5dbcb3e">command list</a> emulation of
            <b>PSSetConstantBuffers1</b> sometimes doesn't actually change the offsets or sizes for the arrays of constant buffers.
            This behavior occurs when <b>PSSetConstantBuffers1</b> doesn't effectively change the constant buffers at the beginning and end of the range of slots that you set to update.
            This section shows how to work around this behavior.
          

Here is the code to check whether either the runtime emulates command lists or the driver supports command lists:
            

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>
     HRESULT hr = S_OK;
     bool needWorkaround = false;
     D3D11_DEVICE_CONTEXT_TYPE contextType = pDeviceContext-&gt;GetType();

     if( D3D11_DEVICE_CONTEXT_DEFERRED == contextType)
     {
          D3D11_FEATURE_DATA_THREADING threadingCaps = { FALSE, FALSE };

          hr = pDevice-&gt;CheckFeatureSupport( D3D11_FEATURE_THREADING, &amp;threadingCaps, sizeof(threadingCaps) );
          if( SUCCEEDED(hr) &amp;&amp; !threadingCaps.DriverCommandLists )
          {
               needWorkaround = true; // the runtime emulates command lists.
          }
     }
</pre>
</td>
</tr>
</table></span></div>
If the runtime emulates command lists, you need to use one of these code snippets:
          

If you change the offset and size on only a single constant buffer, set the constant buffer to <b>NULL</b> first:
            

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>
     pDeviceContext-&gt;PSSetConstantBuffers1(0, 1, &amp;CBuf, &amp;Offset, &amp;Count);
     if( needWorkaround )
     {
          // Workaround for command list emulation
          pDeviceContext-&gt;PSSetConstantBuffers(0, 1, &amp;NullCBuf);
     }
     pDeviceContext-&gt;PSSetConstantBuffers1(0, 1, &amp;CBuf, &amp;Offset, &amp;Count);
</pre>
</td>
</tr>
</table></span></div>
If you change multiple constant buffers, set the first and last constant buffers of the range to <b>NULL</b> first:
            

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>
     pDeviceContext-&gt;PSSetConstantBuffers1(0, 4, &amp;CBufs, &amp;Offsets, &amp;Counts);
     if( needWorkaround )
     {
          // Workaround for command list emulation
          pDeviceContext-&gt;PSSetConstantBuffers(0, 1, &amp;NullCBuf);
          pDeviceContext-&gt;PSSetConstantBuffers(3, 1, &amp;NullCBuf);
     }
     pDeviceContext-&gt;PSSetConstantBuffers1(0, 4, &amp;CBufs, &amp;Offsets, &amp;Counts);
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/DD2A556D-AEF0-407E-A497-CF17ACDEB1A7">ID3D11DeviceContext1</a>
 

 

