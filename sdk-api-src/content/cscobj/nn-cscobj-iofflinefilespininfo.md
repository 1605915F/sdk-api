---
UID: NN:cscobj.IOfflineFilesPinInfo
title: IOfflineFilesPinInfo
author: windows-sdk-content
description: Represents the pinned status of an item in the Offline Files cache.
old-location: of\iofflinefilespininfo.htm
tech.root: offlinefiles
ms.assetid: 529a529a-fbeb-4414-b4c9-46bfcca4aa7a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOfflineFilesPinInfo, IOfflineFilesPinInfo interface [Offline Files], IOfflineFilesPinInfo interface [Offline Files],described, cscobj/IOfflineFilesPinInfo, of.iofflinefilespininfo
ms.topic: interface
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: CscSvc.dll; CscObj.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CscSvc.dll
 - CscObj.dll
api_name:
 - IOfflineFilesPinInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOfflineFilesPinInfo interface


## -description


Represents the pinned status of an item in the Offline Files cache.

When an item is pinned into the Offline Files cache by using the <a href="https://msdn.microsoft.com/6005d755-5e1b-4eba-95a2-b6c9c00b1a64">IOfflineFilesCache::Pin</a> method, it may be pinned for one of the following reasons:
<table>
<tr>
<th>Flag Value</th>
<th>Meaning</th>
</tr>
<tr>
<td><b>OFFLINEFILES_PIN_CONTROL_FLAG_FORUSER</b></td>
<td>This flag is set when a file is pinned using the "Always available offline" option in Windows explorer.</td>
</tr>
<tr>
<td><b>OFFLINEFILES_PIN_CONTROL_FLAG_FORUSER_POLICY</b></td>
<td>This flag is set when a file is pinned by the per-user "Administratively assigned offline files" Group Policy.</td>
</tr>
<tr>
<td><b>OFFLINEFILES_PIN_CONTROL_FLAG_FORALL</b></td>
<td>This flag is set when a file is pinned by the per-computer "Administratively assigned offline files" Group Policy.</td>
</tr>
<tr>
<td><b>OFFLINEFILES_PIN_CONTROL_FLAG_FORREDIR</b></td>
<td>This flag is set when a redirected folder is pinned by Folder Redirection.</td>
</tr>
</table> 

Each of the various <i>IsPinnedForUserXxxxxx</i> methods expresses one of these reasons.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IOfflineFilesPinInfo</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IOfflineFilesPinInfo</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IOfflineFilesPinInfo</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/143cf346-dbe0-42cf-871e-a0cb54722403">IsPinned</a>
</td>
<td align="left" width="63%">
Determines whether the item is pinned.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/67d2c444-2498-4848-a4fb-8cae5ff77eaf">IsPinnedForComputer</a>
</td>
<td align="left" width="63%">
Determines whether the item was pinned for all users on the computer by Group Policy.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b832f75a-3cd4-4421-a0a5-22c5682cb4c3">IsPinnedForFolderRedirection</a>
</td>
<td align="left" width="63%">
Determines whether the item was pinned by Folder Redirection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d0064423-b173-40e5-96c6-dd6dcf05598d">IsPinnedForUser</a>
</td>
<td align="left" width="63%">
Determines whether the item was pinned by a user.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/fa5548e9-0a4e-4e66-a5ea-45d092c239b2">IsPinnedForUserByPolicy</a>
</td>
<td align="left" width="63%">
Determines whether the item was pinned for users by Group Policy.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/9dea396f-ab71-4b2e-b5d3-776c16614f26">Offline Files API Interfaces</a>
 

 

