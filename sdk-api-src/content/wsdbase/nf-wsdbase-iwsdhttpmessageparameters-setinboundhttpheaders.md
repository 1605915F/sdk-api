---
UID: NF:wsdbase.IWSDHttpMessageParameters.SetInboundHttpHeaders
title: IWSDHttpMessageParameters::SetInboundHttpHeaders
author: windows-sdk-content
description: Sets the HTTP headers used for inbound SOAP-over-HTTP transmissions.
old-location: ncd\iwsdhttpmessageparameters_setinboundhttpheaders.htm
tech.root: wsdapi
ms.assetid: fd680016-1e6f-4d15-b1ca-cd2b6b210a71
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWSDHttpMessageParameters interface,SetInboundHttpHeaders method, IWSDHttpMessageParameters.SetInboundHttpHeaders, IWSDHttpMessageParameters::SetInboundHttpHeaders, SetInboundHttpHeaders, SetInboundHttpHeaders method, SetInboundHttpHeaders method,IWSDHttpMessageParameters interface, ncd.iwsdhttpmessageparameters_setinboundhttpheaders, wsdbase/IWSDHttpMessageParameters::SetInboundHttpHeaders
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wsdbase.h
req.include-header: Wsdapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wsdbase.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Wsdapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wsdapi.dll
api_name:
 - IWSDHttpMessageParameters.SetInboundHttpHeaders
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWSDHttpMessageParameters::SetInboundHttpHeaders


## -description


Sets the HTTP headers used for inbound SOAP-over-HTTP transmissions.


## -parameters




### -param pszHeaders [in]

The HTTP headers to be set.


## -returns



Possible return values include, but are not limited to, the following:

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
Method completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The length in characters of <i>pszHeaders</i> exceeds WSD_MAX_TEXT_LENGTH (8192). 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory to complete the operation.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/fae10e9e-0c2b-4817-bd28-a4a85ca180cc">IWSDHttpMessageParameters</a>
 

 

