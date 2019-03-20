---
UID: NN:sbtsv.ITsSbTaskPlugin
title: ITsSbTaskPlugin (sbtsv.h)
author: windows-sdk-content
description: Exposes methods that update the queue of tasks for Remote Desktop Connection Broker plugins.
old-location: termserv\itssbtaskplugin.htm
tech.root: TermServ
ms.assetid: 56463b47-c2f2-43b7-884f-d6fab9bebbf0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITsSbTaskPlugin, ITsSbTaskPlugin interface [Remote Desktop Services], ITsSbTaskPlugin interface [Remote Desktop Services],described, sbtsv/ITsSbTaskPlugin, termserv.itssbtaskplugin
ms.topic: interface
req.header: sbtsv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Sbtsv.idl
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
 - sbtsv.h
api_name:
 - ITsSbTaskPlugin
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITsSbTaskPlugin interface


## -description


Exposes methods that update the queue of tasks for Remote Desktop Connection Broker plugins.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ITsSbTaskPlugin</b> interface inherits from <a href="https://msdn.microsoft.com/db3d3ee7-9e53-4bac-9711-4e85f1016db9">ITsSbPlugin</a>. <b>ITsSbTaskPlugin</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ITsSbTaskPlugin</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/9e8722c4-0070-448a-a97c-aeb1db59ac7b">InitializeTaskPlugin</a>
</td>
<td align="left" width="63%">
Initializes a task that is in the queue of a Remote Desktop Connection Broker plugin.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/a17e4767-5311-4f9b-9d05-cd9e35f7c5e2">SetTaskQueue</a>
</td>
<td align="left" width="63%">
Updates a task in the queue of  a Remote Desktop Connection Broker plugin.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/db3d3ee7-9e53-4bac-9711-4e85f1016db9">ITsSbPlugin</a>



<a href="https://msdn.microsoft.com/150a3c9a-d504-4854-adaa-92e3a7e8ea70">Remote Desktop Virtualization Interfaces</a>
 

 

