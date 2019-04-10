---
UID: NF:wcsplugin.IDeviceModelPlugIn.GetNeutralAxis
title: IDeviceModelPlugIn::GetNeutralAxis (wcsplugin.h)
author: windows-sdk-content
description: The IDeviceModelPlugIn::GetNeutralAxis return the XYZ colorimetry of sample points along the device's neutral axis.
old-location: wcs\IDeviceModelPlugIn_GetNeutralAxis.htm
tech.root: WCS
ms.assetid: 9a3557e0-d533-4357-aa2a-7e168482927a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetNeutralAxis, GetNeutralAxis method [Windows Color System], GetNeutralAxis method [Windows Color System],IDeviceModelPlugIn interface, IDeviceModelPlugIn interface [Windows Color System],GetNeutralAxis method, IDeviceModelPlugIn.GetNeutralAxis, IDeviceModelPlugIn::GetNeutralAxis, _color_IDeviceModelPlugIn::GetNeutralAxis, wcs.IDeviceModelPlugIn_GetNeutralAxis, wcsplugin/IDeviceModelPlugIn::GetNeutralAxis
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
 - IDeviceModelPlugIn.GetNeutralAxis
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDeviceModelPlugIn::GetNeutralAxis


## -description


The <a href="wcs.IDeviceModelPlugIn::GetNeutralAxis">IDeviceModelPlugIn::GetNeutralAxis</a> return the XYZ colorimetry of sample points along the device's neutral axis.


## -parameters




### -param cColors [in]

The number of points that are returned.


### -param pXYZColors [out]

A pointer to an array of <a href="https://msdn.microsoft.com/en-us/library/Dd372458(v=VS.85).aspx">XYZColorF</a> structures.


## -returns



If this function succeeds, the return value is S_OK.

If this function fails, the return value is E_FAIL.




## -remarks



You should define "neutral axis" in a way that is appropriate for your device. Usually, it is points made by the device's gray values. This might be R=G=B, or C=M=Y=0 and any value of K. For some devices, the most pleasing gray may be one that uses a different combination of colorants, such as M=Y=0 and C=K. The plug-in is responsible for determining the colorimetry of a sampling of the neutral axis values and returning them. The sampling may be as sparse as two points (white and black) or as dense as desired.

There is no requirement that the samples be uniformly spaced in any color space.




## -see-also




<a href="https://msdn.microsoft.com/a0623917-0b63-4546-a71a-1e9efa9fe8e5">Basic Color Management Concepts</a>



<a href="https://msdn.microsoft.com/ee9e9502-5514-4070-95fa-265674a1dde7">Functions</a>



<a href="https://msdn.microsoft.com/90541ec2-c0ab-4f98-906b-3e58f8f5cc03">IDeviceModelPlugIn</a>
 

 

