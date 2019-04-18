---
UID: NF:netcon.INetSharingConfiguration.EnableInternetFirewall
title: INetSharingConfiguration::EnableInternetFirewall (netcon.h)
author: windows-sdk-content
description: The EnableInternetFirewall methods enables Internet Connection Firewall on this connection.
old-location: ics\inetsharingconfiguration_enableinternetfirewall.htm
tech.root: ics
ms.assetid: 9805f6bf-ee06-469f-9b2f-e48caa582d1a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EnableInternetFirewall, EnableInternetFirewall method [ICS/ICF], EnableInternetFirewall method [ICS/ICF],INetSharingConfiguration interface, INetSharingConfiguration interface [ICS/ICF],EnableInternetFirewall method, INetSharingConfiguration.EnableInternetFirewall, INetSharingConfiguration::EnableInternetFirewall, _ics_inetsharingconfiguration_enableinternetfirewall, ics.inetsharingconfiguration_enableinternetfirewall, netcon/INetSharingConfiguration::EnableInternetFirewall
ms.topic: method
req.header: netcon.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
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
req.dll: Hnetcfg.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Hnetcfg.dll
api_name:
 - INetSharingConfiguration.EnableInternetFirewall
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# INetSharingConfiguration::EnableInternetFirewall


## -description


<p class="CCE_Message">[Internet Connection Firewall may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/en-us/library/Aa366453(v=VS.85).aspx">Windows Firewall API</a>.]

The 
<b>EnableInternetFirewall</b> methods enables Internet Connection Firewall on this connection.


## -parameters






## -returns



If the method succeeds the return value is S_OK.

If the method fails, the return value is one of the following error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_ABORT</b></dt>
</dl>
</td>
<td width="60%">
The operation was stopped.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unspecified error occurred.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One of the parameters is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOINTERFACE</b></dt>
</dl>
</td>
<td width="60%">
A specified interface is not supported.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
A specified method is not implemented.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
The method was unable to allocate required memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
A pointer passed as a parameter is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
The method failed for unknown reasons.

</td>
</tr>
</table>
 




## -remarks



Calling this method triggers the following notification:

%programname% is attempting to enable Internet Connection Firewall to help protect your computer or network from Internet security threats. However, it may cause some of your older Internet games to function incorrectly. Do you want to turn on Internet Connection Firewall?

Use the 
<a href="https://msdn.microsoft.com/8f774509-0efb-49e5-bf56-61f4810631bd">INetSharingManager::get_INetSharingConfigurationForINetConnection</a> method to obtain an 
<a href="https://msdn.microsoft.com/en-us/library/Aa365935(v=VS.85).aspx">INetSharingConfiguration</a> interface for a particular connection.

<b>Windows XP with SP2:  </b>Calling this API will enable the firewall on the specified interface only when Windows Firewall is enabled.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa365935(v=VS.85).aspx">INetSharingConfiguration</a>



<a href="https://msdn.microsoft.com/dfef918e-9abf-4ac2-8365-28cd5b249add">Internet Connection Sharing and Internet Connection Firewall Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa366131(v=VS.85).aspx">Internet Connection Sharing and Internet Connection Firewall Reference</a>
 

 

