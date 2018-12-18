---
UID: NF:dcomp.IDCompositionDevice.CreateTransform3DGroup
title: IDCompositionDevice::CreateTransform3DGroup
author: windows-sdk-content
description: Creates a 3D transform group object that holds an array of 3D transform objects.
old-location: directcomp\idcompositiondevice_createtransform3dgroup.htm
tech.root: directcomp
ms.assetid: 47119ECA-CAA0-41E7-821E-18E99B6C91BD
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateTransform3DGroup, CreateTransform3DGroup method [DirectComposition], CreateTransform3DGroup method [DirectComposition],IDCompositionDevice interface, IDCompositionDevice interface [DirectComposition],CreateTransform3DGroup method, IDCompositionDevice.CreateTransform3DGroup, IDCompositionDevice::CreateTransform3DGroup, dcomp/IDCompositionDevice::CreateTransform3DGroup, directcomp.idcompositiondevice_createtransform3dgroup
ms.topic: method
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dcomp.lib
req.dll: Dcomp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dcomp.dll
api_name:
 - IDCompositionDevice.CreateTransform3DGroup
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice::CreateTransform3DGroup


## -description


Creates a 3D transform group object that holds an array of 3D transform objects.


## -parameters




### -param transforms3D [in]

Type: <b><a href="https://msdn.microsoft.com/81239AB4-C2A3-4E37-95E3-B3C10532EE15">IDCompositionTransform3D</a>**</b>

An array of 3D transform objects that make up this transform group.


### -param elements [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of elements in the <i>transforms</i> array.


### -param transform3DGroup [out]

Type: <b><a href="https://msdn.microsoft.com/81239AB4-C2A3-4E37-95E3-B3C10532EE15">IDCompositionTransform3D</a>**</b>

The new 3D transform group object. This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



The array entries in a 3D transform group cannot be changed. However, each transform in the array can be modified through its own property setting methods. If a transform in the array is modified, the change is reflected in the computed matrix of the transform group.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh437392(v=VS.85).aspx">IDCompositionDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh437423(v=VS.85).aspx">IDCompositionEffectGroup::SetTransform3D</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449159(v=VS.85).aspx">IDCompositionVisual::SetEffect</a>
 

 

