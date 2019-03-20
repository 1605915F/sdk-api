---
UID: NF:vidcap.ICameraControl.get_IrisRelative
title: ICameraControl::get_IrisRelative (vidcap.h)
author: windows-sdk-content
description: The get_IrisRelative method returns the camera's relative aperture setting. The relative aperture is expressed as a number of steps, where the size of each step depends on the camera model.
old-location: dshow\icameracontrol_get_irisrelative.htm
tech.root: DirectShow
ms.assetid: 15f01c00-ff18-4d58-a03b-9293a8a6a68c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICameraControl interface [DirectShow],get_IrisRelative method, ICameraControl.get_IrisRelative, ICameraControl::get_IrisRelative, ICameraControlget_IrisRelative, dshow.icameracontrol_get_irisrelative, get_IrisRelative, get_IrisRelative method [DirectShow], get_IrisRelative method [DirectShow],ICameraControl interface, vidcap/ICameraControl::get_IrisRelative
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
 - ICameraControl.get_IrisRelative
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICameraControl::get_IrisRelative


## -description


The <code>get_IrisRelative</code> method returns the camera's relative aperture setting. The relative aperture is expressed as a number of steps, where the size of each step depends on the camera model.


## -parameters




### -param pValue [out]

Receives the relative aperture setting. To get the range of possible values, call <a href="https://msdn.microsoft.com/en-us/library/Dd376304(v=VS.85).aspx">ICameraControl::getRange_IrisRelative</a>.

<table>
<tr>
<th>Value
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>0</td>
<td>Default aperture setting.</td>
</tr>
<tr>
<td>Postive value</td>
<td>Open by one step.</td>
</tr>
<tr>
<td>Negative value</td>
<td>Close by one step.</td>
</tr>
</table>
 


### -param pFlags [out]

Receives one or more flags. See <a href="https://msdn.microsoft.com/en-us/library/Dd318251(v=VS.85).aspx">CameraControlFlags</a>.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376298(v=VS.85).aspx">ICameraControl Interface</a>
 

 

