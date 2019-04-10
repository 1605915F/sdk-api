---
UID: NF:wuapi.IUpdate4.get_PerUser
title: IUpdate4::get_PerUser (wuapi.h)
author: windows-sdk-content
description: Gets a Boolean value that indicates whether this is a per-user update.
old-location: wua\iupdate4_peruser.htm
tech.root: Wua_Sdk
ms.assetid: f6d48e78-114f-4926-a1e7-201ac703f8b8
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IUpdate4 interface [Windows Update Agent],PerUser property, IUpdate4.PerUser, IUpdate4.get_PerUser, IUpdate4::PerUser, IUpdate4::get_PerUser, PerUser property [Windows Update Agent], PerUser property [Windows Update Agent],IUpdate4 interface, get_PerUser, wua.iupdate4_peruser, wuapi/IUpdate4::PerUser, wuapi/IUpdate4::get_PerUser
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
 - IUpdate4.PerUser
 - IUpdate4.get_PerUser
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUpdate4::get_PerUser


## -description


Gets a Boolean value that indicates whether this is a per-user update.

This property is read-only.


## -parameters


## -remarks



Per-user updates are  designed to alter the current user’s environment only; not the environment of the machine as a whole. For example, an update which only alters files in the current user’s user directory could be a per-user update; an update which alters files in the Program Files directory or the Windows directory would not be a per-user update. Per-user updates are currently not processed by Automatic Updates or displayed in the Windows Update user interface. Instead, they are only available to callers who specifically request them in searches by using the <a href="https://msdn.microsoft.com/d37017d5-6f78-4b6c-ac0b-c83b83853079">IUpdateSearcher3</a> interface.  On computers running versions of Windows Update Agent that do not implement the <a href="https://msdn.microsoft.com/44904dd6-28d2-46b4-a237-0da68535cc84">IUpdate4</a> interface, only per-machine updates will be available; per-user updates will never be detected.




## -see-also




<a href="https://msdn.microsoft.com/44904dd6-28d2-46b4-a237-0da68535cc84">IUpdate4</a>
 

 

