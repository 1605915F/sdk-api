---
UID: NF:commctrl.ListView_GetGroupCount
title: ListView_GetGroupCount macro (commctrl.h)
author: windows-sdk-content
description: Gets the number of groups. You can use this macro or send the LVM_GETGROUPCOUNT message explicitly.
old-location: controls\ListView_GetGroupCount.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listview\macros\listview_getgroupcount.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ListView_GetGroupCount, ListView_GetGroupCount macro [Windows Controls], _shell_ListView_GetGroupCount, _shell_ListView_GetGroupCount_cpp, commctrl/ListView_GetGroupCount, controls.ListView_GetGroupCount, controls._shell_ListView_GetGroupCount
ms.topic: macro
req.header: commctrl.h
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
 - ListView_GetGroupCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ListView_GetGroupCount macro


## -description


Gets the number of groups. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb774931(v=VS.85).aspx">LVM_GETGROUPCOUNT</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the list-view control. 


## -remarks



To use <b>ListView_GetGroupCount</b>, specify Comctl32.dll version 6 in the manifest. For more information on manifests, see <a href="https://msdn.microsoft.com/en-us/library/Bb773175(v=VS.85).aspx">Enabling Visual Styles</a>. 



