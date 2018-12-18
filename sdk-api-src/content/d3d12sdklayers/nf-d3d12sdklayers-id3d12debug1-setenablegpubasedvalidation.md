---
UID: NF:d3d12sdklayers.ID3D12Debug1.SetEnableGPUBasedValidation
title: ID3D12Debug1::SetEnableGPUBasedValidation
author: windows-sdk-content
description: This method enables or disables GPU-Based Validation (GBV) before creating a device with the debug layer enabled.
old-location: direct3d12\id3d12debugdevice1_setenablegpubasedvalidation.htm
tech.root: direct3d12
ms.assetid: 0B7ACDC1-D7F6-4565-8E33-F2F14A96E4A8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3D12Debug1 interface,SetEnableGPUBasedValidation method, ID3D12Debug1.SetEnableGPUBasedValidation, ID3D12Debug1::SetEnableGPUBasedValidation, SetEnableGPUBasedValidation, SetEnableGPUBasedValidation method, SetEnableGPUBasedValidation method,ID3D12Debug1 interface, d3d12sdklayers/ID3D12Debug1::SetEnableGPUBasedValidation, direct3d12.id3d12debugdevice1_setenablegpubasedvalidation
ms.topic: method
req.header: d3d12sdklayers.h
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
 - COM
api_location:
 - d3d12sdklayers.h
api_name:
 - ID3D12Debug1.SetEnableGPUBasedValidation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12Debug1::SetEnableGPUBasedValidation


## -description


This method enables or disables GPU-Based Validation (GBV) before creating a device with the debug layer enabled.  


## -parameters




### -param Enable

Type: <b>BOOL</b>

TRUE to enable GPU-Based Validation, otherwise FALSE.


## -returns



This method does not return a value.




## -remarks



GPU-Based Validation can only be enabled/disabled prior to creating a device.  By default, GPU-Based Validation is disabled.  To disable GPU-Based Validation after initially enabling it the device must be fully released and recreated.  

For more information, see <a href="https://msdn.microsoft.com/01D1F94F-4DD4-4781-86EF-6C639E8B1069">Using D3D12 Debug Layer GPU-Based Validation</a>.




## -see-also




<a href="https://msdn.microsoft.com/3D69D0CA-5D45-49EA-BCF0-5B0ABB916261">ID3D12Debug1</a>
 

 

