---
UID: NF:faxcomex.IFaxOutboundRouting.GetGroups
title: IFaxOutboundRouting::GetGroups
author: windows-sdk-content
description: The IFaxOutboundRouting::GetGroups method retrieves an interface that represents a collection of outbound routing groups.
old-location: fax\_mfax_faxoutboundrouting_getgroups_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_8j1v_cpp.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetGroups, GetGroups method [Fax Service], GetGroups method [Fax Service],IFaxOutboundRouting interface, IFaxOutboundRouting interface [Fax Service],GetGroups method, IFaxOutboundRouting.GetGroups, IFaxOutboundRouting::GetGroups, _mfax_faxoutboundrouting.getgroups_cpp, fax._mfax_faxoutboundrouting_getgroups_cpp, faxcomex/IFaxOutboundRouting::GetGroups
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcomex.h
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxOutboundRouting.GetGroups
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxOutboundRouting::GetGroups


## -description


The <b>IFaxOutboundRouting::GetGroups</b> method retrieves an interface that represents a collection of outbound routing groups.


## -parameters




### -param pFaxOutboundRoutingGroups [out, retval]

Type: <b><a href="https://msdn.microsoft.com/cf36787b-cc8e-48a8-b81d-5406cbc4bcc8">IFaxOutboundRoutingGroups</a>**</b>

An address of a pointer that receives an <a href="https://msdn.microsoft.com/cf36787b-cc8e-48a8-b81d-5406cbc4bcc8">IFaxOutboundRoutingGroups</a> interface.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To use this method, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farQUERY_CONFIG</a> access right.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms690138(v=VS.85).aspx">IFaxOutboundRouting</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693408(v=VS.85).aspx">Visual Basic Example</a>
 

 

