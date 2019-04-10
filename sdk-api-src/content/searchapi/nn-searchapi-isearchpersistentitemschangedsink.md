---
UID: NN:searchapi.ISearchPersistentItemsChangedSink
title: ISearchPersistentItemsChangedSink (searchapi.h)
author: windows-sdk-content
description: Provides methods for passing change notifications to alert the indexer that items need to be updated.
old-location: search\_search_ISearchPersistentItemsChangedSink.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\notifications\isearchpersistentitemschangedsink\isearchpersistentitemschangedsink.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ISearchPersistentItemsChangedSink, ISearchPersistentItemsChangedSink interface [search], ISearchPersistentItemsChangedSink interface [search],described, _search_ISearchPersistentItemsChangedSink, search._search_ISearchPersistentItemsChangedSink, searchapi/ISearchPersistentItemsChangedSink
ms.topic: interface
req.header: searchapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Searchnotifications.idl
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
 - Searchapi.h
api_name:
 - ISearchPersistentItemsChangedSink
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# ISearchPersistentItemsChangedSink interface


## -description


Provides methods for passing change notifications to alert the indexer that items need to be updated.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ISearchPersistentItemsChangedSink</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>ISearchPersistentItemsChangedSink</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ISearchPersistentItemsChangedSink</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb231455(v=VS.85).aspx">OnItemsChanged</a>
</td>
<td align="left" width="63%">
Notifies the indexer to index changed items.
        

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb231456(v=VS.85).aspx">StartedMonitoringScope</a>
</td>
<td align="left" width="63%">
Called by a notifications provider to notify the indexer to monitor changes to items within a specified hierarchical scope.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb231457(v=VS.85).aspx">StoppedMonitoringScope</a>
</td>
<td align="left" width="63%">
Called by a notifications provider to notify the indexer to stop monitoring changes to items within a specified hierarchical scope.
        

</td>
</tr>
</table> 


## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb266528(v=VS.85).aspx">Notifying the Index of Changes</a>



<a href="https://msdn.microsoft.com/en-us/library/Cc678933(v=VS.85).aspx">The Indexing Process</a>
 

 

