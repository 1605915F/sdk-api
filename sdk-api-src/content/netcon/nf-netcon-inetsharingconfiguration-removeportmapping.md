---
UID: NF:netcon.INetSharingConfiguration.RemovePortMapping
title: INetSharingConfiguration::RemovePortMapping (netcon.h)
author: windows-sdk-content
description: The RemovePortMapping method removes a service port mapping from the list of mappings for this connection.
old-location: ics\inetsharingconfiguration_removeportmapping.htm
tech.root: ics
ms.assetid: 2790aced-a3a9-425d-9e0f-fe8df4fcb934
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: INetSharingConfiguration interface [ICS/ICF],RemovePortMapping method, INetSharingConfiguration.RemovePortMapping, INetSharingConfiguration::RemovePortMapping, RemovePortMapping, RemovePortMapping method [ICS/ICF], RemovePortMapping method [ICS/ICF],INetSharingConfiguration interface, _ics_inetsharingconfiguration_removeportmapping, ics.inetsharingconfiguration_removeportmapping, netcon/INetSharingConfiguration::RemovePortMapping
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
 - INetSharingConfiguration.RemovePortMapping
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# INetSharingConfiguration::RemovePortMapping


## -description


<p class="CCE_Message">[Internet Connection Firewall may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/4043a85f-ebdc-424c-acf5-9097d1472773">Windows Firewall API</a>.]

The 
<b>RemovePortMapping</b> method removes a service port mapping from the list of mappings for this connection.


## -parameters




### -param pMapping [in]

Pointer to an 
<a href="https://msdn.microsoft.com/236608c3-061e-4db0-96df-25d263b6463b">INetSharingPortMapping</a> interface for the port mapping to remove.


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
The operation was aborted.

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
One of the parameters is invalid.

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



Calling this method also removes the name of this port mapping from the list of mappings in the ICS/ICF user interface.

Use the 
<a href="https://msdn.microsoft.com/en-us/library/Aa365966(v=VS.85).aspx">INetSharingManager::get_INetSharingConfigurationForINetConnection</a> method to obtain an 
<a href="https://msdn.microsoft.com/en-us/library/Aa365935(v=VS.85).aspx">INetSharingConfiguration</a> interface for a particular connection.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa365935(v=VS.85).aspx">INetSharingConfiguration</a>



<a href="https://msdn.microsoft.com/0d9e1520-6018-425c-a2f9-c408fa3025cf">INetSharingConfiguration::AddPortMapping</a>



<a href="https://msdn.microsoft.com/f5465acc-2b36-47d1-b48f-b36df3a8efb3">INetSharingConfiguration::EnumPortMappings</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa366128(v=VS.85).aspx">Internet Connection Sharing and Internet Connection Firewall Interfaces</a>



<a href="https://msdn.microsoft.com/7ab18626-adc9-450c-a2b8-723d2c839a7b">Internet Connection Sharing and Internet Connection Firewall Reference</a>
 

 

