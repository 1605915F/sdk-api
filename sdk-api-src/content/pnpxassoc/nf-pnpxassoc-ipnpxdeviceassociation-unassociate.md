---
UID: NF:pnpxassoc.IPNPXDeviceAssociation.Unassociate
title: IPNPXDeviceAssociation::Unassociate
author: windows-sdk-content
description: Marks an association database entry as unassociated and sends an appropriate notification.
old-location: ncd\ipnpxdeviceassociation_unassociate.htm
tech.root: fundisc
ms.assetid: fb420967-c79c-4edd-a432-b982219c0746
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPNPXDeviceAssociation interface,Unassociate method, IPNPXDeviceAssociation.Unassociate, IPNPXDeviceAssociation::Unassociate, Unassociate, Unassociate method, Unassociate method,IPNPXDeviceAssociation interface, ncd.ipnpxdeviceassociation_unassociate, pnpxassoc/IPNPXDeviceAssociation::Unassociate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: pnpxassoc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Pnpxassoc.idl
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
 - pnpxassoc.h
api_name:
 - IPNPXDeviceAssociation.Unassociate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPNPXDeviceAssociation::Unassociate


## -description


<p class="CCE_Message">[Function Discovery is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions.]

Marks an association database entry as unassociated and sends an appropriate notification.


## -parameters




### -param pszSubCategory [in, optional]

The subcategory of the association database in which the entry is stored.  This parameter can be <b>NULL</b>.


### -param pIFunctionDiscoveryNotification [in]

An <a href="https://msdn.microsoft.com/1819fe08-b151-482d-8e2c-1d599fd15609">IFunctionDiscoveryNotification</a> object that is registered for notifications with Function Discovery.  


## -returns



Possible return values include, but are not limited to, the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The method failed.

</td>
</tr>
</table>
 




## -remarks



This method modifies the association database entry corresponding to the function instance from which the <a href="https://msdn.microsoft.com/52669dec-2fd7-4f3e-b322-e93d9da5984d">IPNPXDeviceAssociation</a> interface was obtained. 

The following logic is used to determine the callback method used for notification:

<ul>
<li>If a PnP notification is received after the device is unassociated, then the <a href="https://msdn.microsoft.com/ab4d0fc6-de3f-49cf-b53c-573222a8bc89">IFunctionDiscoveryNotification::OnUpdate</a> method is called  with the <i>enumQueryUpdateAction</i> parameter set to  <b>QUA_REMOVE</b>. </li>
<li>If no PnP notification is received after the device is unassociated, and there are no pending PnP events, then the <a href="https://msdn.microsoft.com/c4dcc4e9-7acf-44d3-b337-1ac01afa19b0">IFunctionDiscoveryNotification::OnError</a> method is called. </li>
<li>Finally, if no PnP notification is received after the device is unassociated, and there are pending PnP events, then no callback method is called.</li>
</ul>
This method does not remove the entry from the association database. To remove an entry from the association database, call <a href="https://msdn.microsoft.com/cc00c135-140d-4e05-9180-779917d88688">IPNPXAssociation::Delete</a>.




## -see-also




<a href="https://msdn.microsoft.com/92f0cc10-03a0-498f-acd1-4b03302aa33b">IPNPXAssociation::Unassociate</a>



<a href="https://msdn.microsoft.com/52669dec-2fd7-4f3e-b322-e93d9da5984d">IPNPXDeviceAssociation</a>
 

 

