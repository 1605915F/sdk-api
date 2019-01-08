---
UID: NS:commctrl.tagTVITEMCHANGE
title: NMTVITEMCHANGE
author: windows-sdk-content
description: Contains information on a tree-view item change. This structure is sent with the TVN_ITEMCHANGED and TVN_ITEMCHANGING notifications.
old-location: controls\NMTVITEMCHANGE.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\structures\nmtvitemchange.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: NMTVITEMCHANGE, NMTVITEMCHANGE structure [Windows Controls], _shell_NMTVITEMCHANGE, _shell_NMTVITEMCHANGE_cpp, commctrl/NMTVITEMCHANGE, controls.NMTVITEMCHANGE, controls._shell_NMTVITEMCHANGE
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
 - NMTVITEMCHANGE
product: Windows
targetos: Windows
req.typenames: NMTVITEMCHANGE
req.redist: 
---

# NMTVITEMCHANGE structure


## -description


Contains information on a tree-view item change. This structure is sent with the <a href="https://msdn.microsoft.com/en-us/library/Bb773526(v=VS.85).aspx">TVN_ITEMCHANGED</a> and <a href="https://msdn.microsoft.com/en-us/library/Bb773530(v=VS.85).aspx">TVN_ITEMCHANGING</a> notifications. 


## -struct-fields




### -field hdr

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a> structure that contains information about the notification.


### -field uChanged

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Specifies the attribute. The only supported attribute is state. <b>uChanged</b> must have the following value:

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
<dt>TVIF_STATE</dt>
</dl>
</td>
<td width="60%">
The change is the state attribute.

</td>
</tr>
</table>
 


### -field hItem

Type: <b>HTREEITEM</b>

Handle to the changed tree-view item.


### -field uStateNew

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Flag that specifies the new item state.


### -field uStateOld

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Flag that specifies the item's previous state.


### -field lParam

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPARAM</a></b>

Reserved for application specific data. For example, a value to associate with the item.

