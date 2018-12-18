---
UID: NF:vidcap.ICameraControl.get_ScanMode
title: ICameraControl::get_ScanMode
author: windows-sdk-content
description: The get_ScanMode method returns the current scanning mode (interlaced or progressive).
old-location: dshow\icameracontrol_get_scanmode.htm
tech.root: DirectShow
ms.assetid: 09a75986-9c5d-44fc-af62-297481854574
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICameraControl interface [DirectShow],get_ScanMode method, ICameraControl.get_ScanMode, ICameraControl::get_ScanMode, ICameraControlget_ScanMode, dshow.icameracontrol_get_scanmode, get_ScanMode, get_ScanMode method [DirectShow], get_ScanMode method [DirectShow],ICameraControl interface, vidcap/ICameraControl::get_ScanMode
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
 - ICameraControl.get_ScanMode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICameraControl::get_ScanMode


## -description


The <code>get_ScanMode</code> method returns the current scanning mode (interlaced or progressive).


## -parameters




### -param pValue [out]

Receives one of the following values.

<table>
<tr>
<th>Value
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>0</td>
<td>Interlaced video.</td>
</tr>
<tr>
<td>1</td>
<td>Progressive video.</td>
</tr>
</table>
 


### -param pFlags [out]

Receives one or more flags. See <a href="https://msdn.microsoft.com/en-us/library/Dd318251(v=VS.85).aspx">CameraControlFlags</a>.


## -returns



Returns an <b>HRESULT</b> value.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376298(v=VS.85).aspx">ICameraControl Interface</a>
 

 

