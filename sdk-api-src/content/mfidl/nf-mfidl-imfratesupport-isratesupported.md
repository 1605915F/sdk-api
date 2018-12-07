---
UID: NF:mfidl.IMFRateSupport.IsRateSupported
title: IMFRateSupport::IsRateSupported
author: windows-sdk-content
description: Queries whether the object supports a specified playback rate.
old-location: mf\imfratesupport_isratesupported.htm
tech.root: medfound
ms.assetid: 3ac04683-17d3-4d87-b260-39b04eab9e59
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 3ac04683-17d3-4d87-b260-39b04eab9e59, IMFRateSupport interface [Media Foundation],IsRateSupported method, IMFRateSupport.IsRateSupported, IMFRateSupport::IsRateSupported, IsRateSupported, IsRateSupported method [Media Foundation], IsRateSupported method [Media Foundation],IMFRateSupport interface, mf.imfratesupport_isratesupported, mfidl/IMFRateSupport::IsRateSupported
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfuuid.lib
 - mfuuid.dll
api_name:
 - IMFRateSupport.IsRateSupported
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFRateSupport::IsRateSupported


## -description



Queries whether the object supports a specified playback rate.




## -parameters




### -param fThin [in]

If <b>TRUE</b>, the method queries whether the object supports the playback rate with thinning. Otherwise, the method queries whether the object supports the playback rate without thinning. For information about thinning, see <a href="https://msdn.microsoft.com/509b2cc8-6017-41a9-ae80-9af21dce9367">About Rate Control</a>.


### -param flRate [in]

The playback rate to query.


### -param pflNearestSupportedRate [in, out]

If the object does not support the playback rate given in <i>flRate</i>, this parameter receives the closest supported playback rate. If the method returns S_OK, this parameter receives the value given in <i>flRate</i>. This parameter can be <b>NULL</b>.


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
The object supports the specified rate.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MF_E_REVERSE_UNSUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The object does not support reverse playback.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MF_E_THINNING_UNSUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The object does not support thinning.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MF_E_UNSUPPORTED_RATE</b></dt>
</dl>
</td>
<td width="60%">
The object does not support the specified rate.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/7f2b64e1-1062-4f77-b8e0-62b6d962ae8b">How to Determine Supported Rates</a>



<a href="https://msdn.microsoft.com/a6c495fa-0f6a-4e4c-8fba-996b22d55053">IMFRateSupport</a>
 

 

