---
UID: NN:cluadmex.IWEExtendWizard
title: IWEExtendWizard
author: windows-sdk-content
description: Implement the IWEExtendWizard interface to add wizard pages to Failover Cluster Administrator's New Resource Wizard or Cluster Application Wizard.
old-location: mscs\iweextendwizard.htm
tech.root: mscs
ms.assetid: 6407163e-a8ca-4601-88a0-ecf87e29b9ab
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWEExtendWizard, IWEExtendWizard interface [Failover Cluster], IWEExtendWizard interface [Failover Cluster],described, _wolf_iweextendwizard, cluadmex/IWEExtendWizard, mscs.iweextendwizard
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
 - IWEExtendWizard
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWEExtendWizard interface


## -description


<p class="CCE_Message">[This interface is available for use in the operating systems specified in the Requirements 
    section. Support for this interface was removed in Windows Server 2008.]

Implement the <b>IWEExtendWizard</b> interface to 
    add wizard pages to <a href="https://msdn.microsoft.com/en-us/library/Aa369060(v=VS.85).aspx">Failover Cluster Administrator's</a> 
    New Resource Wizard or Cluster Application Wizard.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWEExtendWizard</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IWEExtendWizard</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>IWEExtendWizard</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Aa370738(v=VS.85).aspx">CreateWizardPages</a>
</td>
<td align="left" width="63%">
Allows you to create wizard pages and add them to Failover Cluster Administrator's New Resource Wizard or 
      Cluster Application Wizard.

</td>
</tr>
</table> 


## -remarks



To support Wizard97 wizards and wizard pages, implement the 
     <a href="https://msdn.microsoft.com/en-us/library/Aa370728(v=VS.85).aspx">IWEExtendWizard97</a> interface.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa369071(v=VS.85).aspx">Failover Cluster Administrator Extension Interfaces</a>
 

 

