---
UID: NN:qmgr.IBackgroundCopyQMgr
title: IBackgroundCopyQMgr (qmgr.h)
author: windows-sdk-content
description: Use the IBackgroundCopyQMgr interface to create a new group, retrieve an existing group, or enumerate all groups in the queue. A group contains a download job.
old-location: bits\ibackgroundcopyqmgr.htm
tech.root: Bits
ms.assetid: 040662c3-0d96-416a-b5e6-a16a6d3034fc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBackgroundCopyQMgr, IBackgroundCopyQMgr interface [BITS], IBackgroundCopyQMgr interface [BITS],described, bits.ibackgroundcopyqmgr, qmgr/IBackgroundCopyQMgr
ms.topic: interface
req.header: qmgr.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Qmgr.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: QmgrPrxy.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - QmgrPrxy.dll
api_name:
 - IBackgroundCopyQMgr
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBackgroundCopyQMgr interface


## -description


<p class="CCE_Message">[<b>IBackgroundCopyQMgr</b> is available for use in the operating systems specified in the Requirements section.  It may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/72668c9b-e6f3-4f3f-9d4b-50d930d1889d">BITS interfaces</a>.]

Use the <b>IBackgroundCopyQMgr</b> interface to create a new group, retrieve an existing group, or enumerate all groups in the queue. A group contains a download job.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IBackgroundCopyQMgr</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IBackgroundCopyQMgr</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IBackgroundCopyQMgr</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d64fec33-3781-428e-af9d-4a08836760d2">CreateGroup</a>
</td>
<td align="left" width="63%">
Creates a new group and adds it to the queue.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/27cf17e3-b35a-4453-ae0a-8b080fd120dc">EnumGroups</a>
</td>
<td align="left" width="63%">
Enumerates the groups in the queue.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/36836fe5-4858-4c6e-8ce8-1bb71c8e9f5a">GetGroup</a>
</td>
<td align="left" width="63%">
Retrieves an existing group from the queue.

</td>
</tr>
</table> 

