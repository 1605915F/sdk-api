---
UID: NF:commctrl.ListView_GetGroupInfo
title: ListView_GetGroupInfo macro (commctrl.h)
author: windows-sdk-content
description: Gets group information. You can use this macro or send the LVM_GETGROUPINFO message explicitly.
old-location: controls\ListView_GetGroupInfo.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listview\macros\listview_getgroupinfo.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ListView_GetGroupInfo, ListView_GetGroupInfo macro [Windows Controls], _win32_ListView_GetGroupInfo, _win32_ListView_GetGroupInfo_cpp, commctrl/ListView_GetGroupInfo, controls.ListView_GetGroupInfo, controls._win32_ListView_GetGroupInfo
ms.topic: macro
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - HeaderDef
api_location:
 - Commctrl.h
api_name:
 - ListView_GetGroupInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ListView_GetGroupInfo macro


## -description


Gets group information. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb774932(v=VS.85).aspx">LVM_GETGROUPINFO</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the list-view control. 


### -param iGroupId

Type: <b>int</b>


### -param pgrp

Type: <b>PLVGROUP</b>

<a href="https://msdn.microsoft.com/en-us/library/Bb774769(v=VS.85).aspx">LVGROUP</a>

## -remarks



To use <b>ListView_GetGroupInfo</b>, specify Comctl32.dll version 6 in the manifest. For more information on manifests, see <a href="https://msdn.microsoft.com/en-us/library/Bb773175(v=VS.85).aspx">Enabling Visual Styles</a>. 



