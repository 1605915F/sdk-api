---
UID: NE:winuser.POINTER_FEEDBACK_MODE
title: POINTER_FEEDBACK_MODE
author: windows-sdk-content
description: Identifies the visual feedback behaviors available to CreateSyntheticPointerDevice.
old-location: input_pointerdevice\pointer_feedback_mode.htm
tech.root: Input_PointerDevice
ms.assetid: 73D024E9-F83B-408F-BC96-6851AB4603AE
ms.author: windowssdkdev
ms.date: 10/12/2018
ms.keywords: POINTER_FEEDBACK_DEFAULT, POINTER_FEEDBACK_INDIRECT, POINTER_FEEDBACK_MODE, POINTER_FEEDBACK_MODE enumeration, POINTER_FEEDBACK_NONE, input_pointerdevice.pointer_feedback_mode, winuser/POINTER_FEEDBACK_DEFAULT, winuser/POINTER_FEEDBACK_INDIRECT, winuser/POINTER_FEEDBACK_MODE, winuser/POINTER_FEEDBACK_NONE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: winuser.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1809 [desktop apps only]
req.target-min-winversvr: Windows Server [desktop apps only]
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
 - winuser.h
api_name:
 - POINTER_FEEDBACK_MODE
product: Windows
targetos: Windows
req.typenames: POINTER_FEEDBACK_MODE
req.redist: 
---

# POINTER_FEEDBACK_MODE enumeration


## -description


Identifies the visual feedback behaviors available to <a href="https://msdn.microsoft.com/251F837F-DF9A-4A94-B790-73AA7196E4A9">CreateSyntheticPointerDevice</a>.


## -enum-fields




### -field POINTER_FEEDBACK_DEFAULT

Visual feedback might be suppressed by the user's pen (Settings -&gt; Devices -&gt; Pen &amp; Windows Ink) and touch (Settings -&gt; Ease of Access -&gt; Cursor &amp; pointer size) settings.


### -field POINTER_FEEDBACK_INDIRECT

Visual feedback overrides the user's pen and touch settings.


### -field POINTER_FEEDBACK_NONE

Visual feedback is disabled.

