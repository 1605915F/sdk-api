---
UID: NF:vidcap.ICameraControl.put_PanTilt
title: ICameraControl::put_PanTilt (vidcap.h)
author: windows-sdk-content
description: The put_PanTilt method sets the camera's pan and tilt angles.
old-location: dshow\icameracontrol_put_pantilt.htm
tech.root: DirectShow
ms.assetid: d9aa052a-72f9-4a17-bebe-809f43264481
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICameraControl interface [DirectShow],put_PanTilt method, ICameraControl.put_PanTilt, ICameraControl::put_PanTilt, ICameraControlput_PanTilt, dshow.icameracontrol_put_pantilt, put_PanTilt, put_PanTilt method [DirectShow], put_PanTilt method [DirectShow],ICameraControl interface, vidcap/ICameraControl::put_PanTilt
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
 - ICameraControl.put_PanTilt
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICameraControl::put_PanTilt


## -description


The <code>put_PanTilt</code> method sets the camera's pan and tilt angles.


## -parameters




### -param PanValue [in]

Specifies the panning angle, in arc seconds. An arc second is 1/3600th of a degree. See <a href="https://msdn.microsoft.com/en-us/library/Dd376339(v=VS.85).aspx">ICameraControl::put_Pan</a>.


### -param TiltValue [in]

Specifies the tilt angle, in arc seconds. See <a href="https://msdn.microsoft.com/en-us/library/Dd376347(v=VS.85).aspx">ICameraControl::put_Tilt</a>.


### -param Flags [in]

Zero or more flags. See <a href="https://msdn.microsoft.com/en-us/library/Dd318251(v=VS.85).aspx">CameraControlFlags</a>. If the CameraControl_Flags_Auto flag is used, the <i>Value</i> parameter is ignored and the camera sets the default value.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376298(v=VS.85).aspx">ICameraControl Interface</a>
 

 

