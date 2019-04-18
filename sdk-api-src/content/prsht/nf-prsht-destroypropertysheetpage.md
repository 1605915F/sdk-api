---
UID: NF:prsht.DestroyPropertySheetPage
title: DestroyPropertySheetPage function (prsht.h)
author: windows-sdk-content
description: Destroys a property sheet page. An application must call this function for pages that have not been passed to the PropertySheet function.
old-location: controls\DestroyPropertySheetPage.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\propsheet\functions\destroypropertysheetpage.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DestroyPropertySheetPage, DestroyPropertySheetPage function [Windows Controls], _win32_DestroyPropertySheetPage, _win32_DestroyPropertySheetPage_cpp, controls.DestroyPropertySheetPage, controls._win32_DestroyPropertySheetPage, prsht/DestroyPropertySheetPage
ms.topic: function
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
req.lib: Comctl32.lib
req.dll: Comctl32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Comctl32.dll
api_name:
 - DestroyPropertySheetPage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# DestroyPropertySheetPage function


## -description


Destroys a property sheet page. An application must call this function for pages that have not been passed to the <a href="https://msdn.microsoft.com/en-us/library/Bb760811(v=VS.85).aspx">PropertySheet</a> function.


## -parameters




### -param Arg1

Type: <b>HPROPSHEETPAGE</b>

Handle to the property sheet page to delete.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

Returns nonzero if successful, or zero otherwise.



