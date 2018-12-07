---
UID: NN:cluadmex.IWEInvokeCommand
title: IWEInvokeCommand
author: windows-sdk-content
description: Failover Cluster Administrator calls your implementation of the IWEInvokeCommand interface when users select context menu items that you created with the IWEExtendContextMenu interface.
old-location: mscs\iweinvokecommand.htm
tech.root: mscs
ms.assetid: 53997e65-5011-4c3b-9586-ede9ed693ab5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWEInvokeCommand, IWEInvokeCommand interface [Failover Cluster], IWEInvokeCommand interface [Failover Cluster],described, _wolf_iweinvokecommand, cluadmex/IWEInvokeCommand, mscs.iweinvokecommand
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: cluadmex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2003 Enterprise, Windows Server 2003 Datacenter
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: CluAdmEx.idl
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
 - cluadmex.h
api_name:
 - IWEInvokeCommand
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWEInvokeCommand interface


## -description


<p class="CCE_Message">[This interface is available for use in the operating systems specified in the Requirements 
    section. Support for this interface was removed in Windows Server 2008.]

Failover Cluster Administrator calls your implementation of the 
    <b>IWEInvokeCommand</b> interface when users select context 
    menu items that you created with the 
    <a href="https://msdn.microsoft.com/en-us/library/Aa370711(v=VS.85).aspx">IWEExtendContextMenu</a> interface.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWEInvokeCommand</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IWEInvokeCommand</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>IWEInvokeCommand</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa370746(v=VS.85).aspx">InvokeCommand</a>
</td>
<td align="left" width="63%">
Allows you to implement procedures that execute when users select your context menu items.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa369071(v=VS.85).aspx">Failover Cluster Administrator Extension Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa370711(v=VS.85).aspx">IWEExtendContextMenu</a>
 

 

