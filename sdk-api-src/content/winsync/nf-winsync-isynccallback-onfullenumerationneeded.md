---
UID: NF:winsync.ISyncCallback.OnFullEnumerationNeeded
title: ISyncCallback::OnFullEnumerationNeeded
author: windows-sdk-content
description: Occurs when the forgotten knowledge from the source provider is not contained in the current knowledge of the destination provider.
old-location: winsync\isynccallback_onfullenumerationneeded.htm
tech.root: winsync
ms.assetid: f52ddaf2-9ce2-4ebb-bace-024c059b2594
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ISyncCallback interface [Windows Sync],OnFullEnumerationNeeded method, ISyncCallback.OnFullEnumerationNeeded, ISyncCallback::OnFullEnumerationNeeded, OnFullEnumerationNeeded, OnFullEnumerationNeeded method [Windows Sync], OnFullEnumerationNeeded method [Windows Sync],ISyncCallback interface, winsync.isynccallback_onfullenumerationneeded, winsync/ISyncCallback::OnFullEnumerationNeeded
ms.topic: method
req.header: winsync.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - COM
api_location:
 - winsync.h
api_name:
 - ISyncCallback.OnFullEnumerationNeeded
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISyncCallback::OnFullEnumerationNeeded


## -description


Occurs when the forgotten knowledge from the source provider is not contained in the current knowledge of the destination provider.


## -parameters




### -param pFullEnumerationAction [out]

Specifies how a synchronization session should handle the full enumeration.


## -returns



The possible return codes include, but are not limited to, the values shown in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Application-determined error codes.</b></dt>
</dl>
</td>
<td width="60%"></td>
</tr>
</table>
 




## -remarks



By default, if an application callback is not registered to receive this notification, Windows Sync uses <b>SFEA_ABORT</b>.





## -see-also




<a href="https://msdn.microsoft.com/f6c96e02-e9db-402c-8197-580f688b068f">ISyncCallback Interface</a>



<a href="https://msdn.microsoft.com/4fdb7123-d8c8-4ed7-9009-0e772252bbb7">SYNC_FULL_ENUMERATION_ACTION Enumeration</a>
 

 

