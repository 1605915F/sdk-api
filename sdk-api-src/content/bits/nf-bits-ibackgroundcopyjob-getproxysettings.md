---
UID: NF:bits.IBackgroundCopyJob.GetProxySettings
title: IBackgroundCopyJob::GetProxySettings (bits.h)
author: windows-sdk-content
description: Retrieves the proxy information that the job uses to transfer the files.
old-location: bits\ibackgroundcopyjob_getproxysettings.htm
tech.root: Bits
ms.assetid: c2d0ec9b-eaa1-4f78-9ccc-4e91d045cd94
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetProxySettings, GetProxySettings method [BITS], GetProxySettings method [BITS],IBackgroundCopyJob interface, IBackgroundCopyJob interface [BITS],GetProxySettings method, IBackgroundCopyJob.GetProxySettings, IBackgroundCopyJob::GetProxySettings, _drz_ibackgroundcopyjob_getproxysettings, bits.ibackgroundcopyjob_getproxysettings, bits/IBackgroundCopyJob::GetProxySettings
ms.topic: method
req.header: bits.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Bits.lib
req.dll: QmgrPrxy.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - QmgrPrxy.dll
api_name:
 - IBackgroundCopyJob.GetProxySettings
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBackgroundCopyJob::GetProxySettings


## -description


Retrieves the proxy information that the job uses to transfer the files.


## -parameters




### -param pProxyUsage [out]

Specifies the proxy settings the job uses to transfer the files. For a list of proxy options, see the 
<a href="https://msdn.microsoft.com/e066b6c8-905f-4e18-9be7-aa3c134f9e13">BG_JOB_PROXY_USAGE</a> enumeration.


### -param pProxyList [out]

Null-terminated string that contains one or more proxies to use to transfer files. The list is space-delimited. For details on the format of the string, see the Listing Proxy Servers section of 
<a href="https://msdn.microsoft.com/80747c0d-5a09-4ffa-a0ca-b051b82acbf8">Enabling Internet Functionality</a>. Call the 
<a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a> function to free <i>ppProxyList</i> when done.


### -param pProxyBypassList [out]

Null-terminated string that contains an optional list of host names or IP addresses, or both, that were not routed through the proxy. The list is space-delimited. For details on the format of the string, see the Listing the Proxy Bypass section of 
<a href="https://msdn.microsoft.com/80747c0d-5a09-4ffa-a0ca-b051b82acbf8">Enabling Internet Functionality</a>. Call the 
<a href="https://msdn.microsoft.com/en-us/library/windows/desktop/ms680722">CoTaskMemFree</a> function to free <i>ppProxyBypassList</i> when done.


## -returns



This method returns the following <b>HRESULT</b> values, as well as others.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>S_OK</b></b></dt>
</dl>
</td>
<td width="60%">
Proxy information was successfully retrieved.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One or more of the parameters is <b>NULL</b>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/e066b6c8-905f-4e18-9be7-aa3c134f9e13">BG_JOB_PROXY_USAGE</a>



<a href="https://msdn.microsoft.com/fd21a17b-1049-4dd9-a08b-da84699b8006">IBackgroundCopyJob::SetProxySettings</a>
 

 

