---
UID: NF:d3d11sdklayers.ID3D11Debug.ReportLiveDeviceObjects
title: ID3D11Debug::ReportLiveDeviceObjects
author: windows-sdk-content
description: Report information about a device object's lifetime.
old-location: direct3d11\id3d11debug_reportlivedeviceobjects.htm
tech.root: direct3d11
ms.assetid: a4e5f3c1-8b67-488b-8476-464c5ea5abc6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 734af011-a2b7-a89f-361d-01350006a197, ID3D11Debug interface [Direct3D 11],ReportLiveDeviceObjects method, ID3D11Debug.ReportLiveDeviceObjects, ID3D11Debug::ReportLiveDeviceObjects, ReportLiveDeviceObjects, ReportLiveDeviceObjects method [Direct3D 11], ReportLiveDeviceObjects method [Direct3D 11],ID3D11Debug interface, d3d11sdklayers/ID3D11Debug::ReportLiveDeviceObjects, direct3d11.id3d11debug_reportlivedeviceobjects
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d11sdklayers.h
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
 - ID3D11Debug.ReportLiveDeviceObjects
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11Debug::ReportLiveDeviceObjects


## -description


Report information about a device object's lifetime.


## -parameters




### -param Flags

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Ff476205(v=VS.85).aspx">D3D11_RLDO_FLAGS</a></b>

A value from the
            <a href="https://msdn.microsoft.com/en-us/library/Ff476205(v=VS.85).aspx">D3D11_RLDO_FLAGS</a> enumeration.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the following <a href="https://msdn.microsoft.com/en-us/library/Ff476174(v=VS.85).aspx">Direct3D 11 Return Codes</a>.




## -remarks



<b>ReportLiveDeviceObjects</b> uses the value in  <i>Flags</i> to determine the amount of information to report about a device object's lifetime.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff476366(v=VS.85).aspx">ID3D11Debug Interface</a>
 

 

