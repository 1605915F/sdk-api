---
UID: NF:wmsdkidl.IWMReaderNetworkConfig.GetProxySettings
title: IWMReaderNetworkConfig::GetProxySettings
author: windows-sdk-content
description: The GetProxySettings method retrieves the current proxy settings.
old-location: wmformat\iwmreadernetworkconfig_getproxysettings.htm
tech.root: wmformat
ms.assetid: 5fdfc651-05f5-48b3-aeaf-4557c72bc0c0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetProxySettings, GetProxySettings method [windows Media Format], GetProxySettings method [windows Media Format],IWMReaderNetworkConfig interface, IWMReaderNetworkConfig interface [windows Media Format],GetProxySettings method, IWMReaderNetworkConfig.GetProxySettings, IWMReaderNetworkConfig::GetProxySettings, IWMReaderNetworkConfigGetProxySettings, wmformat.iwmreadernetworkconfig_getproxysettings, wmsdkidl/IWMReaderNetworkConfig::GetProxySettings
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IWMReaderNetworkConfig.GetProxySettings
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMReaderNetworkConfig::GetProxySettings


## -description



The <b>GetProxySettings</b> method retrieves the current proxy settings.




## -parameters




### -param pwszProtocol [in]

Pointer to a wide-character null-terminated string containing the protocol.


### -param pProxySetting [out]

Pointer to one member of the <a href="https://msdn.microsoft.com/a055259e-e207-426c-b6ca-a27bc3d0e88c">WMT_PROXY_SETTINGS</a> enumeration type.


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
NULL or invalid argument passed in.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/0957ece7-93fe-411b-b69e-fd03933b09d1">IWMReaderNetworkConfig Interface</a>



<a href="https://msdn.microsoft.com/fe5bc4f2-860a-42e8-b9f1-cd3d8af619c2">IWMReaderNetworkConfig::SetProxySettings</a>
 

 

