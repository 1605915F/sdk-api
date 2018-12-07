---
UID: NF:wuapi.IUpdateHistoryEntry.get_Title
title: IUpdateHistoryEntry::get_Title
author: windows-sdk-content
description: Gets the title of an update.
old-location: wua\iupdatehistoryentry_title.htm
tech.root: wua_sdk
ms.assetid: 8a49fddf-ebaf-403e-bb7f-705ab08395eb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUpdateHistoryEntry interface [Windows Update Agent],Title property, IUpdateHistoryEntry.Title, IUpdateHistoryEntry.get_Title, IUpdateHistoryEntry::Title, IUpdateHistoryEntry::get_Title, Title property [Windows Update Agent], Title property [Windows Update Agent],IUpdateHistoryEntry interface, get_Title, wua.iupdatehistoryentry_title, wuapi/IUpdateHistoryEntry::Title, wuapi/IUpdateHistoryEntry::get_Title
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wuapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional with SP3 [desktop apps only]
req.target-min-winversvr: Windows Server 2003, Windows 2000 Server with SP3 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wuapi.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wuguid.lib
req.dll: Wuapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wuapi.dll
api_name:
 - IUpdateHistoryEntry.Title
 - IUpdateHistoryEntry.get_Title
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUpdateHistoryEntry::get_Title


## -description


Gets the title of an update.

This property is read-only.


## -parameters


## -remarks



The information that   this property returns is for the default user interface (UI) language of the user. However, note the following: 

<ul>
<li>If the default UI language of the user is unavailable, Windows Update Agent (WUA) uses the default UI language of the computer.   </li>
<li>If the default language of the computer is unavailable, WUA uses the language that the provider of the  update recommends.</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/7f67ba11-41b5-4185-a78d-75c76dbe1fbe">IUpdateHistoryEntry</a>



<a href="https://msdn.microsoft.com/7c2a209f-10e8-4158-8201-a062f86b5fdd">IUpdateHistoryEntry.ClientApplicationID</a>
 

 

