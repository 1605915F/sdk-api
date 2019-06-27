---
UID: NF:cscobj.IOfflineFilesEvents.ItemDisconnected
title: IOfflineFilesEvents::ItemDisconnected (cscobj.h)
author: windows-sdk-content
description: Reports that an item in the Offline Files cache has transitioned from online to offline.
old-location: of\iofflinefilesevents_itemdisconnected.htm
tech.root: offlinefiles
ms.assetid: b0f9d873-cda5-4805-bb5e-d23d47b53f1d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IOfflineFilesEvents interface [Offline Files],ItemDisconnected method, IOfflineFilesEvents.ItemDisconnected, IOfflineFilesEvents::ItemDisconnected, ItemDisconnected, ItemDisconnected method [Offline Files], ItemDisconnected method [Offline Files],IOfflineFilesEvents interface, cscobj/IOfflineFilesEvents::ItemDisconnected, of.iofflinefilesevents_itemdisconnected
ms.topic: method
f1_keywords: 
 - "cscobj/IOfflineFilesEvents.ItemDisconnected"
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: CscSvc.dll; CscObj.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CscSvc.dll
 - CscObj.dll
api_name:
 - IOfflineFilesEvents.ItemDisconnected
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOfflineFilesEvents::ItemDisconnected


## -description


Reports that an item in the Offline Files cache has transitioned from online to offline.


## -parameters




### -param pszPath [in]

The item's UNC path string.


### -param ItemType [in]

An <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/cscobj/ne-cscobj-tagofflinefiles_item_type">OFFLINEFILES_ITEM_TYPE</a> enumeration value that indicates the type of the item.


## -returns



The return value is ignored.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/cscobj/nn-cscobj-iofflinefilesevents">IOfflineFilesEvents</a>
 

 

