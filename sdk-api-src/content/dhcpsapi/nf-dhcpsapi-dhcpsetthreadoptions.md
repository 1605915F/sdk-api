---
UID: NF:dhcpsapi.DhcpSetThreadOptions
title: DhcpSetThreadOptions function (dhcpsapi.h)
author: windows-sdk-content
description: The DhcpSetThreadOptions function sets options on the currently executing DHCP thread.
old-location: dhcp\dhcpsetthreadoptions.htm
tech.root: DHCP
ms.assetid: aadca143-6fdd-4b25-9bd5-1ba177be148e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DHCP_FLAGS_DONT_ACCESS_DS, DhcpSetThreadOptions, DhcpSetThreadOptions function [DHCP], dhcp.dhcpsetthreadoptions, dhcpsapi/DhcpSetThreadOptions
ms.topic: function
req.header: dhcpsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008, Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dhcpsapi.lib
req.dll: Dhcpsapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Dhcpsapi.dll
api_name:
 - DhcpSetThreadOptions
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DhcpSetThreadOptions function


## -description


The <b>DhcpSetThreadOptions</b> function sets options on the currently executing DHCP thread.


## -parameters




### -param Flags [in]

Set of bit flags indicating thread settings. If no thread options are  set, the value is 0. Currently, the only bit flag that can be set is as follows.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="DHCP_FLAGS_DONT_ACCESS_DS"></a><a id="dhcp_flags_dont_access_ds"></a><dl>
<dt><b>DHCP_FLAGS_DONT_ACCESS_DS</b></dt>
</dl>
</td>
<td width="60%">
Do not access the directory service while the DHCP thread is executing. After this option is set, the only functions that can access the domain directory service are as follows:

<ul>
<li>
<a href="https://msdn.microsoft.com/c8b4d241-19d4-4a97-9129-c2954d63b6ac">DhcpEnumServers</a>
</li>
<li>
<a href="https://msdn.microsoft.com/bdf5d239-478a-47af-9240-19d1b6933f7e">DhcpAddServer</a>
</li>
<li>
<a href="https://msdn.microsoft.com/88b6c29b-7b01-40c7-b4f5-4920845f1eb9">DhcpDeleteServer</a>
</li>
</ul>
</td>
</tr>
</table>
 


### -param Reserved [in]

Reserved. This parameter must be set to <b>NULL</b>.


## -returns



This function returns <b>ERROR_SUCCESS</b> upon a successful call. Otherwise, it returns one of the <a href="https://msdn.microsoft.com/6370313f-d7db-4ff1-b0e0-7fa47474facb">DHCP Server Management API Error Codes</a>.




## -remarks



<b>DhcpSetThreadOptions</b> currently allows only one option to be set.




## -see-also




<a href="https://msdn.microsoft.com/2ba4b971-467c-47a6-8c4d-8e41b7874c80">DhcpGetThreadOptions</a>
 

 

