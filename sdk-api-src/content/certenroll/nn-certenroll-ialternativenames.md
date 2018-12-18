---
UID: NN:certenroll.IAlternativeNames
title: IAlternativeNames
author: windows-sdk-content
description: Contains methods and properties that enable you to manage a collection of IAlternativeName objects.
old-location: security\ialternativenames.htm
tech.root: seccertenroll
ms.assetid: 6ebd5bd5-7bf3-43e3-9b72-47b2c9743174
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAlternativeNames, IAlternativeNames interface [Security], IAlternativeNames interface [Security],described, certenroll/IAlternativeNames, security.ialternativenames
ms.topic: interface
req.header: certenroll.h
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
req.lib: 
req.dll: CertEnroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CertEnroll.dll
api_name:
 - IAlternativeNames
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAlternativeNames interface


## -description


The <b>IAlternativeNames</b> interface contains methods and properties that enable you to manage a collection of <a href="https://msdn.microsoft.com/2a6cfda8-b3cb-4a0f-bb65-b182c16207be">IAlternativeName</a> objects.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAlternativeNames</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IAlternativeNames</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>IAlternativeNames</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/02085a1c-0821-4b11-95ad-e1c3a69f4e80">Add</a>
</td>
<td align="left" width="63%">
Adds an object to the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/babeb53a-b2db-420c-85fe-dacb9176ec70">Clear</a>
</td>
<td align="left" width="63%">
Removes all objects from the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1507d03b-2c1d-416e-b346-16795902f5e2">Remove</a>
</td>
<td align="left" width="63%">
Removes an object from the collection by index number.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAlternativeNames</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/66656bf5-3258-4888-8c1d-0fde33275504">_NewEnum</a>


</td>
<td align="left" width="63%">
Retrieves the enumerator for the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/ef7f588a-f877-4626-ada6-782db6202c65">Count</a>


</td>
<td align="left" width="63%">
Retrieves the number of objects in the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/778ea065-9a92-4244-be16-23e716ccbb8a">ItemByIndex</a>


</td>
<td align="left" width="63%">
Retrieves an object from the collection by index number.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/d49511ed-8651-457e-a102-0bea4edde24c">CertEnroll Interfaces</a>



<a href="https://msdn.microsoft.com/2a6cfda8-b3cb-4a0f-bb65-b182c16207be">IAlternativeName</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>
 

 

