---
UID: NF:netcon.INetSharingConfiguration.get_EnumPortMappings
title: INetSharingConfiguration::get_EnumPortMappings (netcon.h)
author: windows-sdk-content
description: The get_EnumPortMappings method retrieves an IEnumNetSharingPortMapping interface. Use this interface to enumerate the port mappings for this connection.
old-location: ics\inetsharingconfiguration_enumportmappings.htm
tech.root: ics
ms.assetid: f5465acc-2b36-47d1-b48f-b36df3a8efb3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: INetSharingConfiguration interface [ICS/ICF],get_EnumPortMappings method, INetSharingConfiguration.get_EnumPortMappings, INetSharingConfiguration::get_EnumPortMappings, _ics_inetsharingconfiguration_enumportmappings, get_EnumPortMappings, get_EnumPortMappings method [ICS/ICF], get_EnumPortMappings method [ICS/ICF],INetSharingConfiguration interface, ics.inetsharingconfiguration_enumportmappings, netcon/INetSharingConfiguration::get_EnumPortMappings
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
 - INetSharingConfiguration.get_EnumPortMappings
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# INetSharingConfiguration::get_EnumPortMappings


## -description


<p class="CCE_Message">[Internet Connection Firewall may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/en-us/library/Aa366453(v=VS.85).aspx">Windows Firewall API</a>.]

The 
<b>get_EnumPortMappings</b> method retrieves an 
<a href="https://msdn.microsoft.com/68334bd2-353f-457d-a2c7-1271816f10f5">IEnumNetSharingPortMapping</a> interface. Use this interface to enumerate the port mappings for this connection.


## -parameters




### -param Flags [in]

This parameter must be ICSSC_DEFAULT.


### -param ppColl [out]

Pointer to an interface pointer that, on successful return, points to a 
<a href="https://msdn.microsoft.com/09b91df1-b9ef-41b1-b739-65d95f5d60b1">INetSharingPortMappingCollection</a> interface.


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



Use the 
<a href="https://msdn.microsoft.com/8f774509-0efb-49e5-bf56-61f4810631bd">INetSharingManager::get_INetSharingConfigurationForINetConnection</a> method to obtain an 
<a href="https://msdn.microsoft.com/en-us/library/Aa365935(v=VS.85).aspx">INetSharingConfiguration</a> interface for a particular connection.




## -see-also




<a href="https://msdn.microsoft.com/68334bd2-353f-457d-a2c7-1271816f10f5">IEnumNetSharingPortMapping</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa365935(v=VS.85).aspx">INetSharingConfiguration</a>



<a href="https://msdn.microsoft.com/0d9e1520-6018-425c-a2f9-c408fa3025cf">INetSharingConfiguration::AddPortMapping</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa365954(v=VS.85).aspx">INetSharingConfiguration::RemovePortMapping</a>



<a href="https://msdn.microsoft.com/09b91df1-b9ef-41b1-b739-65d95f5d60b1">INetSharingPortMappingCollection</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa366128(v=VS.85).aspx">Internet Connection Sharing and Internet Connection Firewall Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa366131(v=VS.85).aspx">Internet Connection Sharing and Internet Connection Firewall Reference</a>
 

 

