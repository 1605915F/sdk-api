---
UID: NS:prsht._PSHNOTIFY
title: PSHNOTIFY
author: windows-sdk-content
description: Contains information for the property sheet notification messages.
old-location: controls\PSHNOTIFY.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\propsheet\structures\pshnotify.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPPSHNOTIFY, LPPSHNOTIFY, LPPSHNOTIFY structure pointer [Windows Controls], PSHNOTIFY, PSHNOTIFY structure [Windows Controls], _win32_PSHNOTIFY, _win32_PSHNOTIFY_cpp, controls.PSHNOTIFY, controls._win32_PSHNOTIFY, prsht/LPPSHNOTIFY, prsht/PSHNOTIFY"
ms.topic: struct
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
 - PSHNOTIFY
product: Windows
targetos: Windows
req.typenames: PSHNOTIFY, *LPPSHNOTIFY
req.redist: 
---

# PSHNOTIFY structure


## -description


Contains information for the property sheet notification messages.


## -struct-fields




### -field hdr

Type: <b><a href="https://msdn.microsoft.com/0c8b116b-82ad-495a-b19d-8c172e0b2608">NMHDR</a></b>

Address of an <a href="https://msdn.microsoft.com/0c8b116b-82ad-495a-b19d-8c172e0b2608">NMHDR</a> structure that contains additional information about the notification.


### -field lParam

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPARAM</a></b>

Additional information about this notification. To determine what, if any, information is contained in this member, see the description of the particular notification message.

