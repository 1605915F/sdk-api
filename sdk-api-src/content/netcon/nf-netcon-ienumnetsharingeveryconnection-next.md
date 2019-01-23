---
UID: NF:netcon.IEnumNetSharingEveryConnection.Next
title: IEnumNetSharingEveryConnection::Next
author: windows-sdk-content
description: The Next method retrieves the specified number of connections from the Connections folder starting from the current enumeration position.
old-location: ics\ienumnetsharingeveryconnection_next.htm
tech.root: ics
ms.assetid: 05c1ec04-81bc-4d38-aab5-843ea54dda1d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumNetSharingEveryConnection interface [ICS/ICF],Next method, IEnumNetSharingEveryConnection.Next, IEnumNetSharingEveryConnection::Next, Next, Next method [ICS/ICF], Next method [ICS/ICF],IEnumNetSharingEveryConnection interface, _ics_ienumnetsharingeveryconnection_next, ics.ienumnetsharingeveryconnection_next, netcon/IEnumNetSharingEveryConnection::Next
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
 - IEnumNetSharingEveryConnection.Next
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumNetSharingEveryConnection::Next


## -description


<p class="CCE_Message">[Internet Connection Firewall may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/4043a85f-ebdc-424c-acf5-9097d1472773">Windows Firewall API</a>.]

The 
<b>Next</b> method retrieves the specified number of connections from the Connections folder starting from the current enumeration position.


## -parameters




### -param celt [in]

Specifies the number of privately-shared connections to retrieve.


### -param rgVar [out]

Pointer to a 
<a href="https://msdn.microsoft.com/en-us/library/ms221627(v=VS.85).aspx">VARIANT</a> variable for the connection. This variant contains a pointer to an 
<a href="https://msdn.microsoft.com/en-us/library/Aa365084(v=VS.85).aspx">INetConnection</a> interface.


### -param pceltFetched [out]

Pointer to a <b>ULONG</b> variable that, on successful return, specifies the number of privately-shared connections actually returned.


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
 




## -see-also




<a href="https://msdn.microsoft.com/d3be8047-e0d5-44b7-97d9-536bc4aa11c5">IEnumNetSharingEveryConnection</a>



<a href="https://msdn.microsoft.com/dfef918e-9abf-4ac2-8365-28cd5b249add">Internet Connection Sharing and Internet Connection Firewall Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa366131(v=VS.85).aspx">Internet Connection Sharing and Internet Connection Firewall Reference</a>
 

 

