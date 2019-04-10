---
UID: NF:vidcap.ICameraControl.put_ZoomRelative
title: ICameraControl::put_ZoomRelative (vidcap.h)
author: windows-sdk-content
description: The put_ZoomRelative method sets the camera's relative zoom. The relative zoom indicates the direction in which the lens is moving.
old-location: dshow\icameracontrol_put_zoomrelative.htm
tech.root: DirectShow
ms.assetid: 815f92c3-bfab-47d5-86dd-f9b2321d20eb
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ICameraControl interface [DirectShow],put_ZoomRelative method, ICameraControl.put_ZoomRelative, ICameraControl::put_ZoomRelative, ICameraControlput_ZoomRelative, dshow.icameracontrol_put_zoomrelative, put_ZoomRelative, put_ZoomRelative method [DirectShow], put_ZoomRelative method [DirectShow],ICameraControl interface, vidcap/ICameraControl::put_ZoomRelative
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
 - ICameraControl.put_ZoomRelative
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICameraControl::put_ZoomRelative


## -description


The <code>put_ZoomRelative</code> method sets the camera's relative zoom. The relative zoom indicates the direction in which the lens is moving.


## -parameters




### -param Value [in]

Specifies the relative zoom. The size of the value represents the desired zoom speed; a higher value represents a higher speed. To get the range of possible values, call <a href="https://msdn.microsoft.com/en-us/library/Dd376312(v=VS.85).aspx">ICameraControl::getRange_ZoomRelative</a>.

<table>
<tr>
<th>Value
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>0</td>
<td>Stop zoom lens motion.</td>
</tr>
<tr>
<td>Positive value</td>
<td>Start moving the zoom lens in the telephoto direction (initiate zoom-in).</td>
</tr>
<tr>
<td>Negative value</td>
<td>Start moving the zoom lens in the wide angle direction (initiate zoom-out).</td>
</tr>
</table>
 


### -param Flags [in]

Zero or more flags. See <a href="https://msdn.microsoft.com/en-us/library/Dd318251(v=VS.85).aspx">CameraControlFlags</a>. If the CameraControl_Flags_Auto flag is used, the <i>Value</i> parameter is ignored and the camera sets the default value.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376298(v=VS.85).aspx">ICameraControl Interface</a>
 

 

