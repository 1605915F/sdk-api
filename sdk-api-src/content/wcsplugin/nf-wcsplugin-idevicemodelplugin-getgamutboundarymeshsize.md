---
UID: NF:wcsplugin.IDeviceModelPlugIn.GetGamutBoundaryMeshSize
title: IDeviceModelPlugIn::GetGamutBoundaryMeshSize (wcsplugin.h)
author: windows-sdk-content
description: Returns the required data structure sizes for the GetGamutBoundaryMesh function.
old-location: wcs\IDeviceModelPlugIn_GetGamutBoundaryMeshSize.htm
tech.root: WCS
ms.assetid: 302f8008-c65d-4794-9297-8b47e29e36ce
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetGamutBoundaryMeshSize, GetGamutBoundaryMeshSize method [Windows Color System], GetGamutBoundaryMeshSize method [Windows Color System],IDeviceModelPlugIn interface, IDeviceModelPlugIn interface [Windows Color System],GetGamutBoundaryMeshSize method, IDeviceModelPlugIn.GetGamutBoundaryMeshSize, IDeviceModelPlugIn::GetGamutBoundaryMeshSize, _color_IDeviceModelPlugIn::GetGamutBoundaryMeshSize, wcs.IDeviceModelPlugIn_GetGamutBoundaryMeshSize, wcsplugin/IDeviceModelPlugIn::GetGamutBoundaryMeshSize
ms.topic: method
req.header: wcsplugin.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - WcsPlugIn.h
api_name:
 - IDeviceModelPlugIn.GetGamutBoundaryMeshSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDeviceModelPlugIn::GetGamutBoundaryMeshSize


## -description


Returns the required data structure sizes for the <a href="https://msdn.microsoft.com/en-us/library/Dd372127(v=VS.85).aspx">GetGamutBoundaryMesh</a> function.


## -parameters




### -param pNumVertices [out]

The required number of vertices.


### -param pNumTriangles [out]

The required number of triangles.


## -returns



If this function succeeds, the return value is S_OK.

If the plug-in device model wants WCS to compute its gamut boundary mesh, the return value is S_FALSE.

If this function fails, the return value is E_FAIL.




## -remarks



This function is called by the <a href="https://msdn.microsoft.com/8a40215c-6c37-4346-a669-79b7871f265e">CreateMultiProfileTransform</a> function.




## -see-also




<a href="https://msdn.microsoft.com/a0623917-0b63-4546-a71a-1e9efa9fe8e5">Basic Color Management Concepts</a>



<a href="https://msdn.microsoft.com/ee9e9502-5514-4070-95fa-265674a1dde7">Functions</a>



<a href="https://msdn.microsoft.com/90541ec2-c0ab-4f98-906b-3e58f8f5cc03">IDeviceModelPlugIn</a>
 

 

