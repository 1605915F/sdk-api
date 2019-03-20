---
UID: NF:strmif.IMediaSeeking.SetTimeFormat
title: IMediaSeeking::SetTimeFormat (strmif.h)
author: windows-sdk-content
description: The SetTimeFormat method sets the time format for subsequent seek operations.
old-location: dshow\imediaseeking_settimeformat.htm
tech.root: DirectShow
ms.assetid: b6f64f8a-67b8-4297-8f0d-389001fa1681
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMediaSeeking interface [DirectShow],SetTimeFormat method, IMediaSeeking.SetTimeFormat, IMediaSeeking::SetTimeFormat, IMediaSeekingSetTimeFormat, SetTimeFormat, SetTimeFormat method [DirectShow], SetTimeFormat method [DirectShow],IMediaSeeking interface, dshow.imediaseeking_settimeformat, strmif/IMediaSeeking::SetTimeFormat
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - IMediaSeeking.SetTimeFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMediaSeeking::SetTimeFormat


## -description



The <code>SetTimeFormat</code> method sets the time format for subsequent seek operations.




## -parameters




### -param pFormat [in]

Pointer to a GUID that specifies the time format. See <a href="https://msdn.microsoft.com/510c7146-ff3c-4812-a7ad-b4051aa82ef3">Time Format GUIDs</a>.


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

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
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
Method is not supported.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<b>NULL</b> pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VFW_E_WRONG_STATE</b></dt>
</dl>
</td>
<td width="60%">
Filter graph is not stopped.

</td>
</tr>
</table>
 




## -remarks



This method specifies the time units used by other <b>IMediaSeeking</b> methods, such as <a href="https://msdn.microsoft.com/1b267c02-ec2d-4251-aac7-f2f711b16062">IMediaSeeking::GetPositions</a> and <a href="https://msdn.microsoft.com/aa1369fd-a57a-4246-bb23-969f6ce3cad8">IMediaSeeking::SetPositions</a>. Whenever you call one of these other methods, any parameters that express time values are given in units of the current time format.

The default time format is <a href="https://msdn.microsoft.com/862c95bc-2e0a-42c0-b907-45f64f27bd41">REFERENCE_TIME</a> units (100 nanoseconds). Other time formats include frames, samples, and bytes. To determine if a given format is supported, call the <a href="https://msdn.microsoft.com/443a8dbc-c12a-4d50-9005-1fedf701f6fd">IMediaSeeking::IsFormatSupported</a> method. If a format is supported, you can switch to that format by calling <code>SetTimeFormat</code>. Only one time format is active at any one time.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/32adad53-d1ac-495f-9347-7bdd4ae4b78d">IMediaSeeking Interface</a>



<a href="https://msdn.microsoft.com/aa6dc75e-f124-4404-b8fd-ef227d8cada0">IMediaSeeking::GetTimeFormat</a>



<a href="https://msdn.microsoft.com/16fd71d6-c162-493c-9bca-479d59da5031">IMediaSeeking::QueryPreferredFormat</a>
 

 

