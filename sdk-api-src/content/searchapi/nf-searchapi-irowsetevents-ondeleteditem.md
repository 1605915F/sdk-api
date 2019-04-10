---
UID: NF:searchapi.IRowsetEvents.OnDeletedItem
title: IRowsetEvents::OnDeletedItem (searchapi.h)
author: windows-sdk-content
description: Called by the indexer to notify clients that an item has been deleted. This item may have matched some (or all) of the search criteria for the client rowset.
old-location: search\_search_IRowsetEvents_OnDeletedItem.htm
tech.root: search
ms.assetid: VS|SEARCH|~\search\wds3x\reference\ifaces\querying\irowsetevents\ondeleteditem.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IRowsetEvents interface [search],OnDeletedItem method, IRowsetEvents.OnDeletedItem, IRowsetEvents::OnDeletedItem, OnDeletedItem, OnDeletedItem method [search], OnDeletedItem method [search],IRowsetEvents interface, _search_IRowsetEvents_OnDeletedItem, search._search_IRowsetEvents_OnDeletedItem, searchapi/IRowsetEvents::OnDeletedItem
ms.topic: method
req.header: searchapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Searchquery.idl
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
 - IRowsetEvents.OnDeletedItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRowsetEvents::OnDeletedItem


## -description


Called by the indexer to notify clients that an item has been deleted. This item may have matched some (or all) of the search criteria for the client rowset.
        


## -parameters




### -param itemID [in]

Type: <b>REFPROPVARIANT</b>

Specifies the item in the rowset that has been deleted.
        


### -param deletedItemState [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dd368861(v=VS.85).aspx">ROWSETEVENT_ITEMSTATE</a></b>

Specifies whether the deleted item is currently in the rowset, as a <a href="https://msdn.microsoft.com/en-us/library/Dd368861(v=VS.85).aspx">ROWSETEVENT_ITEMSTATE</a> enumeration.
        


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The <a href="https://msdn.microsoft.com/en-us/library/Dd368861(v=VS.85).aspx">ROWSETEVENT_ITEMSTATE</a> indicates whether or not the item was contained in the original rowset:
        

<ul>
<li><i>ROWSETEVENT_ITEMSTATE_INROWSET</i> indicates that the deleted item is definitely in your rowset.</li>
<li><i>ROWSETEVENT_ITEMSTATE_UNKNOWN</i> indicates that the deleted item may be in your rowset.  The containment status is not known because your rowset is not fully evaluated.</li>
<li><i>ROWSETEVENT_ITEMSTATE_NOTINROWSET</i> indicates the deleted item was definitely not in your original rowset (but may have already been given via an  <a href="https://msdn.microsoft.com/en-us/library/Dd318752(v=VS.85).aspx">OnNewItem</a> or <a href="https://msdn.microsoft.com/en-us/library/Dd318752(v=VS.85).aspx">OnChangedItem</a> event).</li>
</ul>



## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Dd318749(v=VS.85).aspx">IRowsetEvents</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd318747(v=VS.85).aspx">IRowsetPrioritization</a>



<a href="https://msdn.microsoft.com/6cdfb7d3-f849-432c-960f-912e5024c583">Indexing Prioritization and Rowset Events in Windows 7</a>



<a href="https://msdn.microsoft.com/en-us/library/Cc142933(v=VS.85).aspx">PRIORITIZE_FLAGS</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd797839(v=VS.85).aspx">PRIORITY_LEVEL</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd368861(v=VS.85).aspx">ROWSETEVENT_ITEMSTATE</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd368862(v=VS.85).aspx">ROWSETEVENT_TYPE</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Cc465173(v=VS.85).aspx">Rowset Properties</a>
 

 

