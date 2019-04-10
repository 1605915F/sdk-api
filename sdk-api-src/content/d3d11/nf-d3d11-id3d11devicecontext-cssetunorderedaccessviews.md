---
UID: NF:d3d11.ID3D11DeviceContext.CSSetUnorderedAccessViews
title: ID3D11DeviceContext::CSSetUnorderedAccessViews (d3d11.h)
author: windows-sdk-content
description: Sets an array of views for an unordered resource.
old-location: direct3d11\id3d11devicecontext_cssetunorderedaccessviews.htm
tech.root: direct3d11
ms.assetid: 384a15c0-a035-4f83-a927-e2f763e5fb44
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 16820cec-2cc5-1d17-4d7f-118d1fd9660b, CSSetUnorderedAccessViews, CSSetUnorderedAccessViews method [Direct3D 11], CSSetUnorderedAccessViews method [Direct3D 11],ID3D11DeviceContext interface, ID3D11DeviceContext interface [Direct3D 11],CSSetUnorderedAccessViews method, ID3D11DeviceContext.CSSetUnorderedAccessViews, ID3D11DeviceContext::CSSetUnorderedAccessViews, d3d11/ID3D11DeviceContext::CSSetUnorderedAccessViews, direct3d11.id3d11devicecontext_cssetunorderedaccessviews
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
 - ID3D11DeviceContext.CSSetUnorderedAccessViews
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11DeviceContext::CSSetUnorderedAccessViews


## -description


Sets an array of views for an unordered resource.


## -parameters




### -param StartSlot [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index of the first element in the zero-based array to begin setting  (ranges from 0 to D3D11_1_UAV_SLOT_COUNT - 1). D3D11_1_UAV_SLOT_COUNT is defined as 64.


### -param NumUAVs [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Number of views to set (ranges from 0 to D3D11_1_UAV_SLOT_COUNT - <i>StartSlot</i>).
          


### -param ppUnorderedAccessViews [in, optional]

Type: <b><a href="https://msdn.microsoft.com/9def4a7d-f145-4073-8d7d-bf3c7ac7a060">ID3D11UnorderedAccessView</a>*</b>

A pointer to an array of <a href="https://msdn.microsoft.com/9def4a7d-f145-4073-8d7d-bf3c7ac7a060">ID3D11UnorderedAccessView</a> pointers to be set by the method.
          


### -param pUAVInitialCounts [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

An array of append and consume buffer offsets. A value of -1 indicates to keep the current offset. Any other values set the hidden counter
            for that appendable and consumable UAV. <i>pUAVInitialCounts</i> is only relevant for UAVs that were created with either
            <a href="https://msdn.microsoft.com/13cf0083-c61a-478d-94bd-00dec4cf27b7">D3D11_BUFFER_UAV_FLAG_APPEND</a> or <b>D3D11_BUFFER_UAV_FLAG_COUNTER</b> specified
            when the UAV was created; otherwise, the argument is ignored.
          


## -returns



This method does not return a value.




## -remarks



<b>Windows Phone 8:
        </b> This API is supported.
      




## -see-also




<a href="https://msdn.microsoft.com/afb32c09-77f2-4c33-bd93-8dce92a2e45e">ID3D11DeviceContext</a>
 

 

