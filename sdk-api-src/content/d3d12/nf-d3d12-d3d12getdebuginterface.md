---
UID: NF:d3d12.D3D12GetDebugInterface
title: D3D12GetDebugInterface function (d3d12.h)
author: windows-sdk-content
description: Gets a debug interface.
old-location: direct3d12\d3d12getdebuginterface.htm
tech.root: direct3d12
ms.assetid: 6D1D6B73-3C2C-4BE0-B75D-2CD39DAC9499
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: D3D12GetDebugInterface, D3D12GetDebugInterface function, d3d12/D3D12GetDebugInterface, direct3d12.d3d12getdebuginterface
ms.topic: function
req.header: d3d12.h
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
req.lib: D3D12.lib
req.dll: D3D12.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - D3D12.dll
api_name:
 - D3D12GetDebugInterface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# D3D12GetDebugInterface function


## -description


Gets a debug interface.
        


## -parameters




### -param riid [in]

Type: <b>REFIID</b>

The globally unique identifier (<b>GUID</b>) for the debug interface.
            The <b>REFIID</b>, or <b>GUID</b>, of the debug interface can be obtained by using the __uuidof() macro.
            For example, __uuidof(<a href="https://msdn.microsoft.com/6CFAE096-EE09-4DD0-ADA3-A700FD9FDCB9">ID3D12Debug</a>) will get the <b>GUID</b> of the debug interface.
          


### -param ppvDebug [out, optional]

Type: <b>void**</b>

The debug interface, as a pointer to pointer to void.
            See
            <a href="https://msdn.microsoft.com/6CFAE096-EE09-4DD0-ADA3-A700FD9FDCB9">ID3D12Debug</a>and
            <a href="https://msdn.microsoft.com/6FD77F14-E260-4DBB-8434-664DE1F6DE39">ID3D12DebugDevice</a>.
            


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the <a href="https://msdn.microsoft.com/5F6CC962-7DB7-489F-82A4-9388313014D3">Direct3D 12 Return Codes</a>.
          




## -remarks



The function signature PFN_D3D12_GET_DEBUG_INTERFACE is provided as a typedef, so that you can use dynamic linking techniques (<a href="https://msdn.microsoft.com/library/windows/desktop/ms683212(v=vs.85).aspx">GetProcAddress</a>) instead of statically linking.
      


#### Examples

Enable the D3D12 debug layer.


```cpp
// Enable the D3D12 debug layer.
{
    
    ComPtr<ID3D12Debug> debugController;
    if (SUCCEEDED(D3D12GetDebugInterface(IID_PPV_ARGS(&debugController))))
    {
        debugController->EnableDebugLayer();
    }
}

```


Refer to the <a href="https://msdn.microsoft.com/C2323482-D06D-43B7-9BDE-BFB9A6A6B70D">Example Code in the D3D12 Reference</a>.
          

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/C0F9A52C-483D-40B2-9E1F-CB92ADDC2856">Core Functions</a>
 

 

