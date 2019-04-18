---
UID: NF:wmsdkidl.IWMSyncReader.SetOutputSetting
title: IWMSyncReader::SetOutputSetting (wmsdkidl.h)
author: windows-sdk-content
description: The SetOutputSetting method specifies a named setting for a particular output.
old-location: wmformat\iwmsyncreader_setoutputsetting.htm
tech.root: wmformat
ms.assetid: 8deb322f-8b52-46cf-9b5c-76fa34b6bde2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWMSyncReader interface [windows Media Format],SetOutputSetting method, IWMSyncReader.SetOutputSetting, IWMSyncReader::SetOutputSetting, IWMSyncReaderSetOutputSetting, SetOutputSetting, SetOutputSetting method [windows Media Format], SetOutputSetting method [windows Media Format],IWMSyncReader interface, wmformat.iwmsyncreader_setoutputsetting, wmsdkidl/IWMSyncReader::SetOutputSetting
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
 - IWMSyncReader.SetOutputSetting
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWMSyncReader::SetOutputSetting


## -description



The <b>SetOutputSetting</b> method specifies a named setting for a particular output.




## -parameters




### -param dwOutputNum [in]

<b>DWORD</b> containing the output number.


### -param pszName [in]

Pointer to a <b>null</b>-terminated string containing the name of the setting. For a list of global constants representing setting names, see <a href="https://msdn.microsoft.com/effe6c07-e6df-45b0-b865-2a025c466d6f">Output Settings</a>.


### -param Type [in]

Member of the <a href="https://msdn.microsoft.com/en-us/library/Dd757834(v=VS.85).aspx">WMT_ATTR_DATATYPE</a> enumeration type. This value specifies the type of data in the buffer at <i>pValue</i>.


### -param pValue [in]

Pointer to a byte array containing the value of the setting. The type of data stored in this buffer is specified by <i>Type</i>.


### -param cbLength [in]

Size of <i>pValue</i> in bytes.


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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
<i>pszName</i> or <i>pValue</i> is <b>NULL</b>.

OR

<i>dwOutputNum</i> specifies an invalid output number.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
No file is open in the synchronous reader.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>NS_E_INVALID_REQUEST</b></dt>
</dl>
</td>
<td width="60%">
<i>pszName</i> specifies an unsupported setting.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd798576(v=VS.85).aspx">IWMSyncReader Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798593(v=VS.85).aspx">IWMSyncReader::GetOutputSetting</a>
 

 

