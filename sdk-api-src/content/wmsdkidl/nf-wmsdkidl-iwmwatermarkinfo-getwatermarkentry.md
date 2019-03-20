---
UID: NF:wmsdkidl.IWMWatermarkInfo.GetWatermarkEntry
title: IWMWatermarkInfo::GetWatermarkEntry (wmsdkidl.h)
author: windows-sdk-content
description: The GetWatermarkEntry method retrieves information about one available watermarking system.
old-location: wmformat\iwmwatermarkinfo_getwatermarkentry.htm
tech.root: wmformat
ms.assetid: 7f303233-cd20-40ff-b564-4c44bf17a5f4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetWatermarkEntry, GetWatermarkEntry method [windows Media Format], GetWatermarkEntry method [windows Media Format],IWMWatermarkInfo interface, IWMWatermarkInfo interface [windows Media Format],GetWatermarkEntry method, IWMWatermarkInfo.GetWatermarkEntry, IWMWatermarkInfo::GetWatermarkEntry, IWMWatermarkInfoGetWatermarkEntry, wmformat.iwmwatermarkinfo_getwatermarkentry, wmsdkidl/IWMWatermarkInfo::GetWatermarkEntry
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
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
api_name:
 - IWMWatermarkInfo.GetWatermarkEntry
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMWatermarkInfo::GetWatermarkEntry


## -description



The <b>GetWatermarkEntry</b> method retrieves information about one available watermarking system.




## -parameters




### -param wmetType [in]

A value from the <a href="https://msdn.microsoft.com/en-us/library/Dd757881(v=VS.85).aspx">WMT_WATERMARK_ENTRY_TYPE</a> enumeration type specifying the type of watermarking system.


### -param dwEntryNum [in]

<b>DWORD</b> containing the watermark entry number. This number is between zero and one less than the number of watermark entries returned by <a href="https://msdn.microsoft.com/en-us/library/Dd798718(v=VS.85).aspx">IWMWatermarkInfo::GetWatermarkEntryCount</a>.


### -param pEntry [out]

Pointer to a <a href="https://msdn.microsoft.com/en-us/library/Dd757880(v=VS.85).aspx">WMT_WATERMARK_ENTRY</a> structure containing information about the specified watermarking system.


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
</table>
 




## -remarks



No watermarking <a href="https://msdn.microsoft.com/en-us/library/Dd757828(v=VS.85).aspx">DMOs</a> are provided with the Windows Media Format SDK. You can install third-party DMOs to use with your application.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd798716(v=VS.85).aspx">IWMWatermarkInfo Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798718(v=VS.85).aspx">IWMWatermarkInfo::GetWatermarkEntryCount</a>
 

 

