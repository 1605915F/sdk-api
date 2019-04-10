---
UID: NS:d3d10.D3D10_INPUT_ELEMENT_DESC
title: D3D10_INPUT_ELEMENT_DESC (d3d10.h)
author: windows-sdk-content
description: A description of a single element for the input-assembler stage.
old-location: direct3d10\d3d10_input_element_desc.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\d3d10_input_element_desc.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 0181f051-1b3b-7933-88f6-5ddfa2b8cf74, D3D10_INPUT_ELEMENT_DESC, D3D10_INPUT_ELEMENT_DESC structure [Direct3D 10], d3d10/D3D10_INPUT_ELEMENT_DESC, direct3d10.d3d10_input_element_desc
ms.topic: struct
req.header: d3d10.h
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
 - HeaderDef
api_location:
 - D3D10.h
api_name:
 - D3D10_INPUT_ELEMENT_DESC
product: Windows
targetos: Windows
req.typenames: D3D10_INPUT_ELEMENT_DESC
req.redist: 
---

# D3D10_INPUT_ELEMENT_DESC structure


## -description


A description of a single element for the <a href="https://msdn.microsoft.com/en-us/library/Bb205116(v=VS.85).aspx">input-assembler stage</a>.


## -struct-fields




### -field SemanticName

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCSTR</a></b>

The <a href="https://msdn.microsoft.com/en-us/library/Bb509647(v=VS.85).aspx">HLSL semantic</a> associated with this element in a <a href="https://msdn.microsoft.com/en-us/library/Bb509650(v=VS.85).aspx">shader input-signature</a>.


### -field SemanticIndex

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The semantic index for the element. A semantic index modifies a semantic, with an integer index number. A semantic index is only needed in a case where there is more than one element with the same semantic. For example, a 4x4 matrix would have four components each with the semantic name <b>matrix</b>, however each of the four component would have different semantic indices (0, 1, 2, and 3).


### -field Format

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a></b>

The data type of the element data. See <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>.


### -field InputSlot

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

An integer value that identifies the input-assembler (see <a href="https://msdn.microsoft.com/en-us/library/Bb205117(v=VS.85).aspx">input slot</a>). Valid values are between 0 and 15, defined in D3D10.h.


### -field AlignedByteOffset

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Optional. Offset (in bytes) between each element. Use D3D10_APPEND_ALIGNED_ELEMENT for convenience to define the current element directly after the previous one, including any packing if necessary.


### -field InputSlotClass

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205315(v=VS.85).aspx">D3D10_INPUT_CLASSIFICATION</a></b>

Identifies the input data class for a single input slot (see <a href="https://msdn.microsoft.com/en-us/library/Bb205315(v=VS.85).aspx">D3D10_INPUT_CLASSIFICATION</a>).


### -field InstanceDataStepRate

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of instances to draw before stepping one unit forward in a vertex buffer filled with instance data. Can be any unsigned integer value (0 means do not step) when the slot class is D3D10_INPUT_PER_INSTANCE_DATA; must be 0 when the slot class is D3D10_INPUT_PER_VERTEX_DATA.


## -remarks



An input-layout object contains an array of structures, each structure defines one element being read from an input slot. Create an input-layout object by calling <a href="https://msdn.microsoft.com/en-us/library/Bb173550(v=VS.85).aspx">ID3D10Device::CreateInputLayout</a>. For an example, see <a href="https://msdn.microsoft.com/en-us/library/Bb205117(v=VS.85).aspx">Create an input-layout object</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb205153(v=VS.85).aspx">Core Structures</a>
 

 

