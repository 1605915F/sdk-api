---
UID: NS:d3d11.CD3D11_BLEND_DESC
title: CD3D11_BLEND_DESC
author: windows-sdk-content
description: Represents a blend-state structure and provides convenience methods for creating blend-state structures.
old-location: direct3d11\cd3d11_blend_desc.htm
tech.root: direct3d11
ms.assetid: EC45CD9E-FD2E-4D1D-9D35-1CD7C5B8085D
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CD3D11_BLEND_DESC, CD3D11_BLEND_DESC structure [Direct3D 11], d3d11/CD3D11_BLEND_DESC, direct3d11.cd3d11_blend_desc
ms.topic: struct
req.header: d3d11.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - D3D11.h
api_name:
 - CD3D11_BLEND_DESC
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CD3D11_BLEND_DESC structure


## -description


Represents a blend-state structure and provides convenience methods for creating blend-state structures.


## -struct-fields




### -field CD3D11_BLEND_DESC

TBD 


### -field ~CD3D11_BLEND_DESC

TBD 


### -field operator const D3D11_BLEND_DESC&

TBD 


### -field D3D11_BLEND_DESC

 




##### - See Below.


## -remarks



Here is how D3D11.h defines <b>CD3D11_BLEND_DESC</b>:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
struct CD3D11_BLEND_DESC : public D3D11_BLEND_DESC
{
    CD3D11_BLEND_DESC()
    {}
    explicit CD3D11_BLEND_DESC( const D3D11_BLEND_DESC&amp; o ) :
        D3D11_BLEND_DESC( o )
    {}
    explicit CD3D11_BLEND_DESC( CD3D11_DEFAULT )
    {
        AlphaToCoverageEnable = FALSE;
        IndependentBlendEnable = FALSE;
        const D3D11_RENDER_TARGET_BLEND_DESC defaultRenderTargetBlendDesc =
        {
            FALSE,
            D3D11_BLEND_ONE, D3D11_BLEND_ZERO, D3D11_BLEND_OP_ADD,
            D3D11_BLEND_ONE, D3D11_BLEND_ZERO, D3D11_BLEND_OP_ADD,
            D3D11_COLOR_WRITE_ENABLE_ALL,
        };
        for (UINT i = 0; i &lt; D3D11_SIMULTANEOUS_RENDER_TARGET_COUNT; ++i)
            RenderTarget[ i ] = defaultRenderTargetBlendDesc;
    }
    ~CD3D11_BLEND_DESC() {}
    operator const D3D11_BLEND_DESC&amp;() const { return *this; }
};
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/E44951D9-7830-4825-B7FA-CF98CC0D024C">CD3D11 Helper Structures</a>
 

 

