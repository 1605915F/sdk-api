---
UID: NF:wmsdkidl.IWMHeaderInfo.AddMarker
title: IWMHeaderInfo::AddMarker
author: windows-sdk-content
description: The AddMarker method adds a marker, consisting of a name and a specific time, to the header section of the ASF file.
old-location: wmformat\iwmheaderinfo_addmarker.htm
tech.root: wmformat
ms.assetid: cfa111bb-7bbb-448a-b2db-d36637c01a52
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddMarker, AddMarker method [windows Media Format], AddMarker method [windows Media Format],IWMHeaderInfo interface, AddMarker method [windows Media Format],IWMHeaderInfo2 interface, AddMarker method [windows Media Format],IWMHeaderInfo3 interface, IWMHeaderInfo interface [windows Media Format],AddMarker method, IWMHeaderInfo.AddMarker, IWMHeaderInfo2 interface [windows Media Format],AddMarker method, IWMHeaderInfo2::AddMarker, IWMHeaderInfo3 interface [windows Media Format],AddMarker method, IWMHeaderInfo3::AddMarker, IWMHeaderInfo::AddMarker, IWMHeaderInfoAddMarker, wmformat.iwmheaderinfo_addmarker, wmsdkidl/IWMHeaderInfo2::AddMarker, wmsdkidl/IWMHeaderInfo3::AddMarker, wmsdkidl/IWMHeaderInfo::AddMarker
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 7 SDK, or later versions of the SDK
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
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wmvcore.lib
 - Wmvcore.dll
 - WMStubDRM.lib
 - WMStubDRM.dll
 - qasf.dll
api_name:
 - IWMHeaderInfo.AddMarker
 - IWMHeaderInfo2.AddMarker
 - IWMHeaderInfo3.AddMarker
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMHeaderInfo::AddMarker


## -description



The <b>AddMarker</b> method adds a <a href="https://msdn.microsoft.com/en-us/library/Dd757828(v=VS.85).aspx">marker</a>, consisting of a name and a specific time, to the header section of the ASF file.




## -parameters




### -param pwszMarkerName [in]

Pointer to a wide-character null-terminated string containing the marker name. Marker names are limited to 5120 wide characters.


### -param cnsMarkerTime [in]

The marker time in 100-nanosecond increments.


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
<dt><b>NS_E_INVALID_STATE</b></dt>
</dl>
</td>
<td width="60%">
The object cannot currently be configured.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<i>pwszMarkerName</i> is not a valid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
The method failed for an unspecified reason.

</td>
</tr>
</table>
 




## -remarks



The writer does not support markers. When accessing <b>IWMheaderInfo</b> from the writer, calls to <b>AddMarker</b> will return E_NOTIMPL.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd798504(v=VS.85).aspx">IWMHeaderInfo Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798505(v=VS.85).aspx">IWMHeaderInfo2</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798508(v=VS.85).aspx">IWMHeaderInfo3</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798521(v=VS.85).aspx">IWMHeaderInfo::GetMarker</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798525(v=VS.85).aspx">IWMHeaderInfo::RemoveMarker</a>



<a href="https://msdn.microsoft.com/ba9bc93e-76a9-4a49-951f-c38dbcceef8c">Markers</a>
 

 

