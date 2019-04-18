---
UID: NN:bdaiface.IBDA_IPSinkInfo
title: IBDA_IPSinkInfo (bdaiface.h)
author: windows-sdk-content
description: This interface is available for use in the Microsoft Windows 2000, Windows XP, and Windows Server 2003 operating systems.
old-location: mstv\ibda_ipsinkinfo.htm
tech.root: mstv
ms.assetid: fbbe12ea-964a-4a83-ac0a-ac8808bd9a63
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IBDA_IPSinkInfo, IBDA_IPSinkInfo interface [Microsoft TV Technologies], IBDA_IPSinkInfo interface [Microsoft TV Technologies],described, IBDA_IPSinkInfoInterface, bdaiface/IBDA_IPSinkInfo, mstv.ibda_ipsinkinfo
ms.topic: interface
req.header: bdaiface.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - COM
api_location:
 - bdaiface.h
api_name:
 - IBDA_IPSinkInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IBDA_IPSinkInfo interface


## -description



This interface is available for use in the Microsoft Windows 2000, Windows XP, and Windows Server 2003 operating systems. It may be altered or unavailable in subsequent versions.
        

The <b>IBDA_IPSinkInfo</b> interface is implemented on the <a href="https://msdn.microsoft.com/78cd6cba-3bd7-4ad4-b65d-c6b866a18d4e">BDA IP Sink</a> filter, which manages the delivery of in-band IP data to the network stack. This interface supersedes <a href="https://msdn.microsoft.com/en-us/library/Dd693375(v=VS.85).aspx">IBDA_IPSinkControl</a>.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IBDA_IPSinkInfo</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IBDA_IPSinkInfo</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IBDA_IPSinkInfo</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693379(v=VS.85).aspx">get_AdapterDescription</a>
</td>
<td align="left" width="63%">
Retrieves the description of the network adapter.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693380(v=VS.85).aspx">get_AdapterIPAddress</a>
</td>
<td align="left" width="63%">
Retrieves the IP address of the data that the IP Sink filter receives.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693381(v=VS.85).aspx">get_MulticastList</a>
</td>
<td align="left" width="63%">
Retrieves a list of the multicast addresses to which the IP Sink filter is listening.

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IBDA_IPSinkInfo)</code>.




## -see-also




<a href="https://msdn.microsoft.com/07d18f73-e852-4c88-a2e2-e8f4198ca799">BDA Interfaces</a>
 

 

