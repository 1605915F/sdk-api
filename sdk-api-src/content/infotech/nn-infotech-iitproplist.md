---
UID: NN:infotech.IITPropList
title: IITPropList
author: windows-sdk-content
description: Use this interface to set properties for build objects such as word wheels and indexes. Call these methods in the document build process to define properties for all build objects.
old-location: htmlhelp\iitproplist.htm
tech.root: htmlhelp
ms.assetid: VS|htmlhelp|~\html\refiitproplistinterface.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IITPropList, IITPropList interface [HTML Help Workshop], IITPropList interface [HTML Help Workshop],described, htmlhelp.iitproplist, infotech/IITPropList, refIITPropListInterface
ms.topic: interface
req.header: infotech.h
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
 - Infotech.h
api_name:
 - IITPropList
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IITPropList interface


## -description


Use this interface to set properties for build objects such as word wheels and indexes. Call these methods in the document build process to define properties for all build objects.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IITPropList</b> interface inherits from <b>IPersistStreamInit</b>. <b>IITPropList</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IITPropList</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670036(v=VS.85).aspx">Clear</a>
</td>
<td align="left" width="63%">
Clears memory associated with a property list and reinitializes the list.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670037(v=VS.85).aspx">Get</a>
</td>
<td align="left" width="63%">
Returns the property object associated with the given property ID.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/83d9fa7b-d814-4293-93b9-9454c01c1503">GetDataSize</a>
</td>
<td align="left" width="63%">
Returns the number of bytes needed to save the property data. 

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670038(v=VS.85).aspx">GetFirst</a>
</td>
<td align="left" width="63%">
Returns the first property object in a property list.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/73206149-cbc3-475d-8dc8-bb7547f41173">GetHeaderSize</a>
</td>
<td align="left" width="63%">
Returns the number of bytes needed to save the header. 

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670041(v=VS.85).aspx">SaveData</a>
</td>
<td align="left" width="63%">
Saves the data size and data from the property list to a buffer.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670042(v=VS.85).aspx">SaveHeader</a>
</td>
<td align="left" width="63%">
Saves the property ID and data type from the property list to a buffer. Only saves properties marked with a persistence state of TRUE.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670043(v=VS.85).aspx">Set(PROPID,DWORD,DWORD)</a>
</td>
<td align="left" width="63%">
Sets a property to a given value or deletes a property from the list.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670047(v=VS.85).aspx">Set(PROPID,LPCWSTR,DWORD)</a>
</td>
<td align="left" width="63%">
Sets a property to a given value or deletes a property from the list.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670046(v=VS.85).aspx">Set(PROPID,LPVOID,DWORD,DWORD)</a>
</td>
<td align="left" width="63%">
Sets a property to a given value or deletes a property from the list.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670044(v=VS.85).aspx">SetPersist(BOOL)</a>
</td>
<td align="left" width="63%">
Sets the persistence state on or off for all properties.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms670045(v=VS.85).aspx">SetPersist(PROPID,BOOL)</a>
</td>
<td align="left" width="63%">
Sets the persistence state on or off for a given property.



</td>
</tr>
</table> 

