---
UID: NF:vidcap.ICameraControl.getRange_Exposure
title: ICameraControl::getRange_Exposure (vidcap.h)
author: windows-sdk-content
description: The getRange_Exposure method returns the range of exposure times supported by the camera.
old-location: dshow\icameracontrol_getrange_exposure.htm
tech.root: DirectShow
ms.assetid: 42e74ae3-6a07-47c8-8e6a-daf2cb32328c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ICameraControl interface [DirectShow],getRange_Exposure method, ICameraControl.getRange_Exposure, ICameraControl::getRange_Exposure, ICameraControlgetRange_Exposure, dshow.icameracontrol_getrange_exposure, getRange_Exposure, getRange_Exposure method [DirectShow], getRange_Exposure method [DirectShow],ICameraControl interface, vidcap/ICameraControl::getRange_Exposure
ms.topic: method
req.header: vidcap.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - ICameraControl.getRange_Exposure
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICameraControl::getRange_Exposure


## -description


The <code>getRange_Exposure</code> method returns the range of exposure times supported by the camera.


## -parameters




### -param pMin [out]

Receives the minimum exposure time, in log base 2 seconds. If the value is <i>n</i>, the exposure time is 2^n seconds.


### -param pMax [out]

Receives the maximum exposure time, in log base 2 seconds.


### -param pSteppingDelta [out]

Receives the smallest step between settings.


### -param pDefault [out]

Receives the default exposure time.


### -param pCapsFlag [out]

Receives one or more flags. See <a href="https://msdn.microsoft.com/en-us/library/Dd318251(v=VS.85).aspx">CameraControlFlags</a>.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376298(v=VS.85).aspx">ICameraControl Interface</a>
 

 

