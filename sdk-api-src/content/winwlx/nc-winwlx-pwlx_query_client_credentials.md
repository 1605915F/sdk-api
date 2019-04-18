---
UID: NC:winwlx.PWLX_QUERY_CLIENT_CREDENTIALS
title: PWLX_QUERY_CLIENT_CREDENTIALS (winwlx.h)
author: windows-sdk-content
description: Called by a replacement GINA DLL if Terminal Services is enabled. GINA calls this function to retrieve the credentials of remote Terminal Services clients that are not using an Internet connector license.
old-location: security\wlxqueryclientcredentials.htm
tech.root: SecAuthN
ms.assetid: b563606d-f4d5-48d7-914d-a11ed5f536a1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: PWLX_QUERY_CLIENT_CREDENTIALS, PWLX_QUERY_CLIENT_CREDENTIALS callback, WlxQueryClientCredentials, WlxQueryClientCredentials callback function [Security], _gina_wlxqueryclientcredentials, security.wlxqueryclientcredentials, winwlx/WlxQueryClientCredentials
ms.topic: callback
req.header: winwlx.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - winwlx.h
api_name:
 - WlxQueryClientCredentials
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# PWLX_QUERY_CLIENT_CREDENTIALS callback function


## -description


<p class="CCE_Message">[The WlxQueryClientCredentials function is no longer available for use as of Windows Server 2008 and Windows Vista.]

The <b>WlxQueryClientCredentials</b> function is called by a replacement GINA DLL if Terminal Services is enabled.
<div class="alert"><b>Note</b>   GINA DLLs are ignored in Windows Vista.</div><div> </div><a href="https://msdn.microsoft.com/c9567a5b-bd56-4ae1-9eac-af0bb5a6842a">GINA</a> calls this function to retrieve the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">credentials</a> of remote Terminal Services clients that are not using an Internet connector license.

The GINA DLL can use this information to fill in a logon box automatically and attempt to log the user in.


## -parameters




### -param pCred [out]

Specifies a pointer to a 
<a href="https://msdn.microsoft.com/25fdc00d-e484-415f-8f1b-1f8ed911f9ef">WLX_CLIENT_CREDENTIALS_INFO_V1_0</a> structure that contains the credentials of the client on return.


## -returns



The <b>WlxQueryClientCredentials</b> function returns one of the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TRUE</b></dt>
</dl>
</td>
<td width="60%">
The credentials information was retrieved and returned in <i>pCred</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>FALSE</b></dt>
</dl>
</td>
<td width="60%">
The credentials information was not retrieved.

</td>
</tr>
</table>
 




## -remarks



The GINA DLL is responsible for calling 
<a href="https://msdn.microsoft.com/a0393983-cb43-4dfa-91a6-d82a5fb8de12">LocalFree</a> to free the resources used by this structure when the structure is no longer needed.

In order to access this function, the GINA DLL must use the 
<a href="https://msdn.microsoft.com/47e343b8-ee54-45de-98c6-0ec75b45aa90">WLX_DISPATCH_VERSION_1_3</a> structure, and set the Winlogon version to at least WLX_VERSION_1_3 in its 
<a href="https://msdn.microsoft.com/9e7bab30-5cc6-4c55-82e4-d888e1af59ed">WlxNegotiate</a> call.

If the Terminal Services client is using an Internet connector license, the GINA DLL must call 
<a href="https://msdn.microsoft.com/dfa12961-1552-4531-8f79-d44fb2a46e74">WlxQueryInetConnectorCredentials</a>.

Other Winlogon support functions that may be called when Terminal Services is enabled are <a href="https://msdn.microsoft.com/4f9f56dd-13cf-4125-90d0-4858a6c141be">WlxDisconnect</a>, <a href="https://msdn.microsoft.com/dfa12961-1552-4531-8f79-d44fb2a46e74">WlxQueryInetConnectorCredentials</a>, and <a href="https://msdn.microsoft.com/bb36254c-0696-4f3f-89d7-332837ec3a75">WlxWin31Migrate</a>.




## -see-also




<a href="https://msdn.microsoft.com/47e343b8-ee54-45de-98c6-0ec75b45aa90">WLX_DISPATCH_VERSION_1_3</a>



<a href="https://msdn.microsoft.com/4f9f56dd-13cf-4125-90d0-4858a6c141be">WlxDisconnect</a>



<a href="https://msdn.microsoft.com/9e7bab30-5cc6-4c55-82e4-d888e1af59ed">WlxNegotiate</a>



<a href="https://msdn.microsoft.com/dfa12961-1552-4531-8f79-d44fb2a46e74">WlxQueryInetConnectorCredentials</a>



<a href="https://msdn.microsoft.com/bb36254c-0696-4f3f-89d7-332837ec3a75">WlxWin31Migrate</a>
 

 

