---
UID: NF:searchapi.ISearchManager.get_PortNumber
title: ISearchManager::get_PortNumber (searchapi.h)
author: windows-sdk-content
description: Retrieves the port number used to communicate with the proxy server. This port number is stored in the indexer and is set by the ISearchManager::SetProxy method.
old-location: search\_search_ISearchManager_get_PortNumber.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\indexmanagement\isearchmanager\get_portnumber.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ISearchManager interface [search],get_PortNumber method, ISearchManager.get_PortNumber, ISearchManager::get_PortNumber, _search_ISearchManager_get_PortNumber, get_PortNumber, get_PortNumber method [search], get_PortNumber method [search],ISearchManager interface, search._search_ISearchManager_get_PortNumber, searchapi/ISearchManager::get_PortNumber
ms.topic: method
req.header: searchapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Searchadmin.idl
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
 - ISearchManager.get_PortNumber
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
ms.custom: 19H1
---

# ISearchManager::get_PortNumber


## -description


Retrieves the port number used to communicate with the proxy server. This port number is stored in the indexer and is set by the <a href="https://msdn.microsoft.com/en-us/library/Bb231488(v=VS.85).aspx">ISearchManager::SetProxy</a> method.


## -parameters




### -param pdwPortNumber [out, retval]

Type: <b>DWORD*</b>

Receives a pointer to the port number.
            


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The ReindexMatchingUrls code sample, available on <a href="http://go.microsoft.com/fwlink/p/?linkid=155654">Code Gallery</a> and the <a href="http://go.microsoft.com/fwlink/p/?linkid=129787">Windows 7 SDK</a>, demonstrates ways to specify which files to re-index and how.



