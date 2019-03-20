---
UID: NF:wmsdkidl.IWMWriter.SetOutputFilename
title: IWMWriter::SetOutputFilename (wmsdkidl.h)
author: windows-sdk-content
description: The SetOutputFilename method specifies the name of the file to be written.
old-location: wmformat\iwmwriter_setoutputfilename.htm
tech.root: wmformat
ms.assetid: 352cf497-f7d6-41e8-bdbb-c59215b617a3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMWriter interface [windows Media Format],SetOutputFilename method, IWMWriter.SetOutputFilename, IWMWriter::SetOutputFilename, IWMWriterSetOutputFilename, SetOutputFilename, SetOutputFilename method [windows Media Format], SetOutputFilename method [windows Media Format],IWMWriter interface, wmformat.iwmwriter_setoutputfilename, wmsdkidl/IWMWriter::SetOutputFilename
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
api_name:
 - IWMWriter.SetOutputFilename
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMWriter::SetOutputFilename


## -description



The <b>SetOutputFilename</b> method specifies the name of the file to be written.




## -parameters




### -param pwszFilename [in]

Pointer to a wide-character null-terminated string containing the file name.


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
The method failed for an unspecified reason.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>NS_E_INVALID_STATE</b></dt>
</dl>
</td>
<td width="60%">
The writer is not in a configurable state.

</td>
</tr>
</table>
 




## -remarks



This method is equivalent to creating a file sink with an index of 0 and adding it through a call to <a href="https://msdn.microsoft.com/en-us/library/Dd798727(v=VS.85).aspx">IWMWriterAdvanced::AddSink</a>, and is provided for convenience.

You can obtain a pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd757467(v=VS.85).aspx">IWMWriterSink</a> interface of the file sink created by this method by calling <a href="https://msdn.microsoft.com/en-us/library/Dd798728(v=VS.85).aspx">IWMWriterAdvanced::GetSink</a>. This is important because the writer does not deliver status messages for the sinks associated with it. You can call <b>QueryInterface</b> on <b>IWMWriterSink</b> to obtain a pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd743613(v=VS.85).aspx">IWMRegisterCallback</a>, which is used to set an <a href="https://msdn.microsoft.com/en-us/library/Dd798545(v=VS.85).aspx">IWMStatusCallback::OnStatus</a> callback method to which the sink will deliver status messages.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd798719(v=VS.85).aspx">IWMWriter Interface</a>



<a href="https://msdn.microsoft.com/0cc4320a-c975-452d-bd1c-394d43bd4585">Using File Sinks</a>
 

 

