---
UID: NF:videoacc.IAMVideoAccelerator.GetInternalMemInfo
title: IAMVideoAccelerator::GetInternalMemInfo (videoacc.h)
author: windows-sdk-content
description: The GetInternalMemInfo method queries for the amount of scratch memory the hardware abstraction layer (HAL) will allocate for its private use.
old-location: dshow\iamvideoaccelerator_getinternalmeminfo.htm
tech.root: DirectShow
ms.assetid: 64b6371c-4baf-4ec1-bd0d-6413f053e2fa
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetInternalMemInfo, GetInternalMemInfo method [DirectShow], GetInternalMemInfo method [DirectShow],IAMVideoAccelerator interface, IAMVideoAccelerator interface [DirectShow],GetInternalMemInfo method, IAMVideoAccelerator.GetInternalMemInfo, IAMVideoAccelerator::GetInternalMemInfo, IAMVideoAcceleratorGetInternalMemInfo, dshow.iamvideoaccelerator_getinternalmeminfo, videoacc/IAMVideoAccelerator::GetInternalMemInfo
ms.topic: method
req.header: videoacc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IAMVideoAccelerator.GetInternalMemInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMVideoAccelerator::GetInternalMemInfo


## -description



The <b>GetInternalMemInfo</b> method queries for the amount of scratch memory the hardware abstraction layer (HAL) will allocate for its private use. 




## -parameters




### -param pGuid [in]

Pointer to a GUID that specifies the DXVA profile in use.
          


### -param pamvaUncompDataInfo [in]

Pointer to an <a href="https://msdn.microsoft.com/en-us/library/Dd373449(v=VS.85).aspx">AMVAUncompDataInfo</a> structure that specifies the size and pixel format of the uncompressed data.


### -param pamvaInternalMemInfo [in, out]

Pointer to an <a href="https://msdn.microsoft.com/en-us/library/Dd373447(v=VS.85).aspx">AMVAInternalMemInfo</a> structure that receives the amount of scratch memory the HAL will allocate. 


## -returns



Returns an <b>HRESULT</b> value that depends on the implementation of the interface. <b>HRESULT</b> can include one of the following standard constants, or other values not listed.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
Failure.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Argument is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
Method is not supported.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<b>NULL</b> pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/0bc6b65b-4502-4c6f-a0f2-82a2bd444d1d">How Decoders Use IAMVideoAccelerator</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd375992(v=VS.85).aspx">IAMVideoAccelerator Interface</a>
 

 

