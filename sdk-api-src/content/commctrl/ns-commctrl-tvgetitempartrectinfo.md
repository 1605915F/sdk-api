---
UID: NS:commctrl.tagTVGETITEMPARTRECTINFO
title: TVGETITEMPARTRECTINFO
author: windows-sdk-content
description: Contains information for identifying the &#0034;hit zone&#0034; for a specified part of a tree item. The structure is used with the TVM_GETITEMPARTRECT message and the TreeView_GetItemPartRect macro.
old-location: controls\TVGETITEMPARTRECTINFO.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\structures\tvgetitempartrectinfo.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TVGETITEMPARTRECTINFO, TVGETITEMPARTRECTINFO structure [Windows Controls], _shell_TVGETITEMPARTRECTINFO, _shell_TVGETITEMPARTRECTINFO_cpp, commctrl/TVGETITEMPARTRECTINFO, controls.TVGETITEMPARTRECTINFO, controls._shell_TVGETITEMPARTRECTINFO
ms.topic: struct
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
 - TVGETITEMPARTRECTINFO
product: Windows
targetos: Windows
req.typenames: TVGETITEMPARTRECTINFO
req.redist: 
---

# TVGETITEMPARTRECTINFO structure


## -description


Contains information for identifying the "hit zone" for a specified part of a tree item. The structure is used with the <a href="https://msdn.microsoft.com/4fa5d167-9649-4346-89c2-8a48e8d4d2f6">TVM_GETITEMPARTRECT</a> message and the <a href="https://msdn.microsoft.com/1a0175dc-5ce9-472e-91bc-b58a087b0e77">TreeView_GetItemPartRect</a> macro.


## -struct-fields




### -field hti

Type: <b>HTREEITEM</b>

Handle to the parent item.


### -field prc

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a>*</b>

Pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure to receive the coordinates of the bounding rectangle. The sender of the message (the caller) is responsible for allocating this structure.


### -field partID

Type: <b>TVITEMPART</b>

ID of the item part. This value must be <b>TVGIPR_BUTTON</b> (0x0001).

