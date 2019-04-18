---
UID: NN:comsvcs.ICrmMonitorClerks
title: ICrmMonitorClerks (comsvcs.h)
author: windows-sdk-content
description: Retrieves information about the state of clerks.
old-location: cos\icrmmonitorclerks.htm
tech.root: cossdk
ms.assetid: 90403516-f677-4396-8991-ae621c159567
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ICrmMonitorClerks, ICrmMonitorClerks interface [COM+], ICrmMonitorClerks interface [COM+],described, _dtc_ICrmMonitorClerks_Interface, comsvcs/ICrmMonitorClerks, cos.icrmmonitorclerks
ms.topic: interface
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - ComSvcs.h
api_name:
 - ICrmMonitorClerks
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ICrmMonitorClerks interface


## -description


Retrieves information about the state of clerks.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ICrmMonitorClerks</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>ICrmMonitorClerks</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ICrmMonitorClerks</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/19a242a6-ce21-4ce5-984e-cc2220476e2b">ActivityId</a>
</td>
<td align="left" width="63%">
Retrieves the activity ID of the CRM Worker for the specified index.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/3603d898-1601-419b-b3f8-3ad49f2070a0">Description</a>
</td>
<td align="left" width="63%">
Retrieves the description of the CRM Compensator for the specified index.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/bbebfa75-7ca1-46fb-b246-7f3c312987fa">get__NewEnum</a>
</td>
<td align="left" width="63%">
Retrieves an enumerator for the instance CLSIDs of the CRM clerks.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/677f39e5-6f77-46a5-9429-682c0d2933df">get_Count</a>
</td>
<td align="left" width="63%">
Retrieves the count of CRM clerks in the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/af25d159-95e6-4695-9350-9a3c1bc034e9">Item</a>
</td>
<td align="left" width="63%">
Retrieves the instance CLSID of the CRM clerk for the specified index.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c174908b-293e-4481-b35d-455ee4f52eea">ProgIdCompensator</a>
</td>
<td align="left" width="63%">
Retrieves the ProgId of the CRM Compensator for the specified index.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/9907ae75-7cb6-4fde-837c-616b106b4d7d">TransactionUOW</a>
</td>
<td align="left" width="63%">
Retrieves the unit of work (UOW) of the transaction for the specified index.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/3d490da6-1577-4a77-9f7d-6188f96f2914">COM+ Compensating Resource Manager</a>
 

 

