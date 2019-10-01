---
UID: NF:searchapi.IEnumSearchRoots.Reset
title: IEnumSearchRoots::Reset (searchapi.h)
author: windows-sdk-content
description: Moves the internal counter to the beginning of the list so a subsequent call to IEnumSearchRoots::Next retrieves from the beginning.
old-location: search\_search_IEnumSearchRoots_Reset.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\crawlscope\ienumsearchroots\reset.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IEnumSearchRoots interface [search],Reset method, IEnumSearchRoots.Reset, IEnumSearchRoots::Reset, Reset, Reset method [search], Reset method [search],IEnumSearchRoots interface, _search_IEnumSearchRoots_Reset, search._search_IEnumSearchRoots_Reset, searchapi/IEnumSearchRoots::Reset
ms.topic: method
f1_keywords: 
 - "searchapi/IEnumSearchRoots.Reset"
req.header: searchapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
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
 - Searchapi.h
api_name:
 - IEnumSearchRoots.Reset
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
ms.custom: 19H1
---

# IEnumSearchRoots::Reset


## -description


Moves the internal counter to the beginning of the list so a subsequent call to <a href="https://docs.microsoft.com/windows/desktop/api/searchapi/nf-searchapi-ienumsearchroots-next">IEnumSearchRoots::Next</a> retrieves from the beginning.
        


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<b>Windows 7 and later</b>: the CrawlScopeCommandLine code sample, available on <a href="http://go.microsoft.com/fwlink/p/?linkid=155654">Code Gallery</a> and the <a href="http://go.microsoft.com/fwlink/p/?linkid=129787">Windows 7 SDK</a>, demonstrates how to define command line options for Crawl Scope Manager (CSM) indexing operations.
        



