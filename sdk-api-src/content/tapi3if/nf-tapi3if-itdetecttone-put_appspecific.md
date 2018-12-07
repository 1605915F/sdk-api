---
UID: NF:tapi3if.ITDetectTone.put_AppSpecific
title: ITDetectTone::put_AppSpecific
author: windows-sdk-content
description: The put_AppSpecific method sets the application-defined tag that identifies the tone to detect.
old-location: tapi3\itdetecttone_put_appspecific.htm
tech.root: tapi
ms.assetid: 0d008cda-bb01-4249-a0ca-a40d2daacbc4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITDetectTone interface [TAPI 2.2],put_AppSpecific method, ITDetectTone.put_AppSpecific, ITDetectTone::put_AppSpecific, _tapi3_itdetecttone_put_appspecific, put_AppSpecific, put_AppSpecific method [TAPI 2.2], put_AppSpecific method [TAPI 2.2],ITDetectTone interface, tapi3.itdetecttone_put_appspecific, tapi3if/ITDetectTone::put_AppSpecific
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tapi3if.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITDetectTone.put_AppSpecific
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITDetectTone::put_AppSpecific


## -description


The 
<b>put_AppSpecific</b> method sets the application-defined tag that identifies the tone to detect.


## -parameters




### -param lAppSpecific [in]

Specifies an application-specific tag that identifies the tone to detect. When the TAPI Server detects the tone, the value of this parameter is passed back to the application in the <b>TE_TONEEVENT</b> event.


## -returns



This method can return one of these values.

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
Method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/c03db3e2-3dc9-443f-8acf-66c06940e0b9">ITDetectTone</a>



<a href="https://msdn.microsoft.com/a3ffba50-664d-42d2-87b2-fe6943715e85">get_AppSpecific</a>
 

 

