---
UID: NN:taskschd.ITaskNamedValueCollection
title: ITaskNamedValueCollection
author: windows-sdk-content
description: Contains a collection of ITaskNamedValuePair interface name-value pairs.
old-location: taskschd\itasknamedvaluecollection.htm
tech.root: taskschd
ms.assetid: 440dc70b-02de-4974-ad2a-462491d12775
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITaskNamedValueCollection, ITaskNamedValueCollection interface [Task Scheduler], ITaskNamedValueCollection interface [Task Scheduler],described, taskschd.itasknamedvaluecollection, taskschd/ITaskNamedValueCollection
ms.topic: interface
req.header: taskschd.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Taskschd.lib
req.dll: Taskschd.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - taskschd.dll
api_name:
 - ITaskNamedValueCollection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITaskNamedValueCollection interface


## -description


Contains a collection of <a href="https://msdn.microsoft.com/b9d186a3-017d-409e-9d67-e74dc69a486a">ITaskNamedValuePair</a> interface name-value pairs.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ITaskNamedValueCollection</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>ITaskNamedValueCollection</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>ITaskNamedValueCollection</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ac6ac365-5315-49d4-b67a-9c840a2caf51">Clear</a>
</td>
<td align="left" width="63%">
Clears the entire collection of name-value pairs.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/aec5ca20-b983-48e1-a5d0-761f18557fe4">Create</a>
</td>
<td align="left" width="63%">
Creates a name-value pair in the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7c73fb37-5551-497f-86d9-b7158109ca38">Remove</a>
</td>
<td align="left" width="63%">
Removes a selected name-value pair from the collection.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ITaskNamedValueCollection</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="10%">Access type</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/53bcb237-939e-4e10-bc83-83a5dcdeab70">_NewEnum</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
Gets the collection enumerator for the name-value pair collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/aedb4d3d-0f72-4224-8488-4100d2416994">Count</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
Gets the number of name-value pairs in the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/a243b814-7d83-466d-bd49-3414f3240780">Item</a>


</td>
<td align="left" width="10%">
Read-only

</td>
<td align="left" width="63%">
Gets the specified name-value pair from the collection.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/e7b822a0-1e5e-4dd2-8139-ac44c6308fe0">HeaderFields Property of IEmailAction</a>



<a href="https://msdn.microsoft.com/0bceb9d5-11f3-40a3-ba05-be896420e1db">ValueQueries Property of IEventTrigger</a>
 

 

