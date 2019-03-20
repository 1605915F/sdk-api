---
UID: NF:sensorsapi.ISensor.GetState
title: ISensor::GetState (sensorsapi.h)
author: windows-sdk-content
description: Retrieves the current operational state of the sensor.
old-location: winsensors_com_ref\isensor_getstate.htm
tech.root: SensorsAPI
ms.assetid: ec8683a5-f2b3-48ce-8732-16429ee16a7f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetState, GetState method, GetState method,ISensor interface, ISensor interface,GetState method, ISensor.GetState, ISensor::GetState, sensorsapi/ISensor::GetState, winsensors_com_ref.isensor_getstate
ms.topic: method
req.header: sensorsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Sensorsapi.lib
req.dll: Sensorsapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - sensorsapi.dll
api_name:
 - ISensor.GetState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISensor::GetState


## -description


Retrieves the current operational state of the sensor.


## -parameters




### -param pState [out]

Address of a <a href="https://msdn.microsoft.com/en-us/library/Dd318905(v=VS.85).aspx">SensorState</a> variable that receives the current state.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
The sensor driver did not provide a state value. The value provided through <i>pState</i> is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
NULL was passed in for pState.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/3216afbb-d524-486d-99ad-0ee0cfb884e0">ISensor</a>
 

 

