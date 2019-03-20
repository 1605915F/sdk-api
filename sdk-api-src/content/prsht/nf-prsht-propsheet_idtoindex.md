---
UID: NF:prsht.PropSheet_IdToIndex
title: PropSheet_IdToIndex macro (prsht.h)
author: windows-sdk-content
description: Takes the resource identifier (ID) of a property sheet page and returns its zero-based index. You can use this macro or send the PSM_IDTOINDEX message explicitly.
old-location: controls\PropSheet_IdToIndex.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\propsheet\macros\propsheet_idtoindex.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PropSheet_IdToIndex, PropSheet_IdToIndex macro [Windows Controls], _win32_PropSheet_IdToIndex, _win32_PropSheet_IdToIndex_cpp, controls.PropSheet_IdToIndex, controls._win32_PropSheet_IdToIndex, prsht/PropSheet_IdToIndex
ms.topic: macro
req.header: prsht.h
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
 - Prsht.h
api_name:
 - PropSheet_IdToIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PropSheet_IdToIndex macro


## -description


Takes the resource identifier (ID) of a property sheet page and returns its zero-based index. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb774583(v=VS.85).aspx">PSM_IDTOINDEX</a> message explicitly.


## -parameters




### -param hDlg

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the property sheet window.


### -param id

Type: <b>int</b>

Resource ID of the page.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb774656(v=VS.85).aspx">PropSheet_IndexToId</a>
 

 

