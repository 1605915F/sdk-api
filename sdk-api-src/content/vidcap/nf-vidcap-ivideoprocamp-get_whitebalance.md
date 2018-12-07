---
UID: NF:vidcap.IVideoProcAmp.get_WhiteBalance
title: IVideoProcAmp::get_WhiteBalance
author: windows-sdk-content
description: The get_WhiteBalance method returns the camera's white balance, specified as a color temperature.
old-location: dshow\ivideoprocamp_get_whitebalance.htm
tech.root: DirectShow
ms.assetid: 53743bff-4257-4abf-b41a-aa5586ab37b5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVideoProcAmp interface [DirectShow],get_WhiteBalance method, IVideoProcAmp.get_WhiteBalance, IVideoProcAmp::get_WhiteBalance, IVideoProcAmpget_WhiteBalance, dshow.ivideoprocamp_get_whitebalance, get_WhiteBalance, get_WhiteBalance method [DirectShow], get_WhiteBalance method [DirectShow],IVideoProcAmp interface, vidcap/IVideoProcAmp::get_WhiteBalance
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IVideoProcAmp.get_WhiteBalance
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVideoProcAmp::get_WhiteBalance


## -description


The <code>get_WhiteBalance</code> method returns the camera's white balance, specified as a color temperature.


## -parameters




### -param pValue [out]

Receives the white balance, in degrees Kelvin.


### -param pFlags [out]

Receives one or more flags. See <a href="https://msdn.microsoft.com/42876f3b-d2b9-4ddb-85c0-80f5177eef6b">VideoProcAmpFlags</a>.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/efaef34a-688a-4c7d-b8ee-e0f52468e355">IVideoProcAmp Interface</a>
 

 

