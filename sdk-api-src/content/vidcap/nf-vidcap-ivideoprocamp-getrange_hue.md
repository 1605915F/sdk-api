---
UID: NF:vidcap.IVideoProcAmp.getRange_Hue
title: IVideoProcAmp::getRange_Hue (vidcap.h)
author: windows-sdk-content
description: The getRange_Hue method returns the range of hue settings supported by the camera.
old-location: dshow\ivideoprocamp_getrange_hue.htm
tech.root: DirectShow
ms.assetid: 5625b73c-8033-4930-af26-e7c4b4fb6516
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVideoProcAmp interface [DirectShow],getRange_Hue method, IVideoProcAmp.getRange_Hue, IVideoProcAmp::getRange_Hue, IVideoProcAmpgetRange_Hue, dshow.ivideoprocamp_getrange_hue, getRange_Hue, getRange_Hue method [DirectShow], getRange_Hue method [DirectShow],IVideoProcAmp interface, vidcap/IVideoProcAmp::getRange_Hue
ms.topic: method
req.header: vidcap.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
 - Vidcap.h
api_name:
 - IVideoProcAmp.getRange_Hue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVideoProcAmp::getRange_Hue


## -description


The <code>getRange_Hue</code> method returns the range of hue settings supported by the camera.


## -parameters




### -param pMin [out]

Receives the minimum hue setting.


### -param pMax [out]

Receives the maximum hue setting.


### -param pSteppingDelta [out]

Receives the smallest step between settings.


### -param pDefault [out]

Receives the default hue setting.


### -param pCapsFlag [out]

Receives one or more flags. See <a href="https://msdn.microsoft.com/en-us/library/Dd407327(v=VS.85).aspx">VideoProcAmpFlags</a>.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd377236(v=VS.85).aspx">IVideoProcAmp Interface</a>
 

 

