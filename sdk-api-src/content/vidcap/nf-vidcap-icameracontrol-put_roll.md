---
UID: NF:vidcap.ICameraControl.put_Roll
title: ICameraControl::put_Roll
author: windows-sdk-content
description: The put_Roll method sets the camera's roll angle.
old-location: dshow\icameracontrol_put_roll.htm
tech.root: DirectShow
ms.assetid: f74c7acc-e141-4238-bcbe-7890646e706c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICameraControl interface [DirectShow],put_Roll method, ICameraControl.put_Roll, ICameraControl::put_Roll, ICameraControlput_Roll, dshow.icameracontrol_put_roll, put_Roll, put_Roll method [DirectShow], put_Roll method [DirectShow],ICameraControl interface, vidcap/ICameraControl::put_Roll
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ICameraControl.put_Roll
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICameraControl::put_Roll


## -description


The <code>put_Roll</code> method sets the camera's roll angle.


## -parameters




### -param Value [in]

Specifies the roll angle, in degrees. Positive values are clockwise along the image viewing axis, and negative values are counter clockwise. Theoretical values range from –180 degrees to +180 degrees, but the actual range depends on the camera. See <a href="https://msdn.microsoft.com/14400765-d8a2-4ac2-a26b-39949ecd2bda">ICameraControl::getRange_Roll</a>.


### -param Flags [in]

Zero or more flags. See <a href="https://msdn.microsoft.com/806322e7-9a70-4dc1-8b10-2479fb3ec935">CameraControlFlags</a>. If the CameraControl_Flags_Auto flag is used, the <i>Value</i> parameter is ignored and the camera sets the default value.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/7046f96d-a613-4056-84dd-be022efdda4f">ICameraControl Interface</a>
 

 

