---
UID: NF:vidcap.IVideoProcAmp.put_DigitalMultiplier
title: IVideoProcAmp::put_DigitalMultiplier (vidcap.h)
author: windows-sdk-content
description: The put_DigitalMultiplier method sets the camera's digital zoom level.
old-location: dshow\ivideoprocamp_put_digitalmultiplier.htm
tech.root: DirectShow
ms.assetid: c1832aad-22fc-41f0-a99a-09b56c148384
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVideoProcAmp interface [DirectShow],put_DigitalMultiplier method, IVideoProcAmp.put_DigitalMultiplier, IVideoProcAmp::put_DigitalMultiplier, IVideoProcAmpput_DigitalMultiplier, dshow.ivideoprocamp_put_digitalmultiplier, put_DigitalMultiplier, put_DigitalMultiplier method [DirectShow], put_DigitalMultiplier method [DirectShow],IVideoProcAmp interface, vidcap/IVideoProcAmp::put_DigitalMultiplier
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
 - IVideoProcAmp.put_DigitalMultiplier
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVideoProcAmp::put_DigitalMultiplier


## -description


The <code>put_DigitalMultiplier</code> method sets the camera's digital zoom level.


## -parameters




### -param Value [in]

Specifies the digital zoom multiplier.


### -param Flags [in]

Zero or more flags. See <a href="https://msdn.microsoft.com/en-us/library/Dd407327(v=VS.85).aspx">VideoProcAmpFlags</a>. If the VideoProcAmp_Flags_Auto flag is used, the <i>Value</i> parameter is ignored and the camera sets the default value.


## -returns



Returns an <b>HRESULT</b> value.




## -remarks



For more information about the digital zoom multiplier, see <a href="https://msdn.microsoft.com/en-us/library/Dd377254(v=VS.85).aspx">IVideoProcAmp::get_DigitalMultiplier</a>.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd377236(v=VS.85).aspx">IVideoProcAmp Interface</a>
 

 

