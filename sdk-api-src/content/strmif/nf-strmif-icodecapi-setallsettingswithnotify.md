---
UID: NF:strmif.ICodecAPI.SetAllSettingsWithNotify
title: ICodecAPI::SetAllSettingsWithNotify
author: windows-sdk-content
description: The SetAllSettingsWithNotify method reads codec properties from a stream, sets them on the codec, and returns a list of the properties that changed.
old-location: dshow\icodecapi_setallsettingswithnotify.htm
tech.root: DirectShow
ms.assetid: 30f840d1-4c73-4a76-ba0b-c04f2901ad76
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICodecAPI interface [DirectShow],SetAllSettingsWithNotify method, ICodecAPI.SetAllSettingsWithNotify, ICodecAPI::SetAllSettingsWithNotify, ICodecAPISetAllSettingsWithNotify, SetAllSettingsWithNotify, SetAllSettingsWithNotify method [DirectShow], SetAllSettingsWithNotify method [DirectShow],ICodecAPI interface, dshow.icodecapi_setallsettingswithnotify, strmif/ICodecAPI::SetAllSettingsWithNotify
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps \| UWP apps]
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
 - ICodecAPI.SetAllSettingsWithNotify
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICodecAPI::SetAllSettingsWithNotify


## -description



The <b>SetAllSettingsWithNotify</b> method reads codec properties from a stream, sets them on the codec, and returns a list of the properties that changed.




## -parameters




### -param __MIDL__ICodecAPI0002 [in]

Pointer to the <b>IStream</b> interface of the stream.


### -param ChangedParam [out]

Receives a pointer to an array of GUIDs. The array contains the GUIDs of any properties that changed as a result of this method call. The caller must free the array by calling <b>CoTaskMemFree</b>.
          


### -param ChangedParamCount [in]

Receives the number of elements in the <i>ChangedParam</i> array.
          


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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
Not implemented.

</td>
</tr>
</table>
 




## -remarks



Codecs that implement <a href="https://msdn.microsoft.com/cc3f1bd9-1d36-45e6-94e2-07f2800fd073">ICodecAPI</a> are  not required to support this method.




## -see-also




<a href="https://msdn.microsoft.com/82085fd5-2d31-48a0-b2ef-0eede4de60c8">Codec API Reference</a>



<a href="https://msdn.microsoft.com/3d19152f-17a3-4576-a2a2-5b827d9ca8d1">Encoder API</a>



<a href="https://msdn.microsoft.com/cc3f1bd9-1d36-45e6-94e2-07f2800fd073">ICodecAPI</a>



<a href="https://msdn.microsoft.com/863ba518-c3c6-47d8-96d8-445a7e4d02aa">ICodecAPI::GetValue</a>
 

 

