---
UID: NS:d3d11_1.D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA
title: D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA
author: windows-sdk-content
description: Represents key exchange data for hardware content protection.
old-location: mf\d3d11_key_exchange_hw_protection_data.htm
tech.root: medfound
ms.assetid: 1DAAE15F-80E4-4645-8326-0ECB1809F8CF
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA, D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA structure [Media Foundation], d3d11_1/D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA, mf.d3d11_key_exchange_hw_protection_data
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3d11_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - d3d11_1.h
api_name:
 - D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA
product: Windows
targetos: Windows
req.typenames: D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA
req.redist: 
---

# D3D11_KEY_EXCHANGE_HW_PROTECTION_DATA structure


## -description


Represents key exchange data for hardware content protection.


## -struct-fields




### -field HWProtectionFunctionID

The function ID of the DRM command. The values and meanings of the function ID are defined by the DRM specification.


### -field pInputData

Pointer to a buffer containing a <a href="https://msdn.microsoft.com/en-us/library/Dn894116(v=VS.85).aspx">D3D11_KEY_EXCHANGE_HW_PROTECTION_INPUT_DATA</a> structure that specifies memory reserved for IHV use and the input data for the DRM command.


### -field pOutputData

Pointer to a buffer containing a <a href="https://msdn.microsoft.com/en-us/library/Dn894117(v=VS.85).aspx">D3D11_KEY_EXCHANGE_HW_PROTECTION_OUTPUT_DATA</a> structure that specifies memory reserved for IHV use and the input data for the DRM command.


### -field Status

The result of the hardware DRM command.


## -remarks



A pointer to this structure is passed in the <i>pData</i> parameter of <a href="https://msdn.microsoft.com/en-us/library/Hh447714(v=VS.85).aspx">ID3D11VideoContext::NegotiateCryptoSessionKeyExchange</a> method when the <a href="https://msdn.microsoft.com/en-us/library/Hh447691(v=VS.85).aspx">ID3D11CryptoSession</a> is creating using the <b>D3D11_KEY_EXCHANGE_HW_PROTECTION</b> key exchange type.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh447680(v=VS.85).aspx">Direct3D 11 Video Structures</a>
 

 

