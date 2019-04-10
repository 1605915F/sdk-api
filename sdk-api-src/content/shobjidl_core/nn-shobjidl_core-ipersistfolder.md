---
UID: NN:shobjidl_core.IPersistFolder
title: IPersistFolder (shobjidl_core.h)
author: windows-sdk-content
description: Exposes a method that initializes Shell folder objects.
old-location: shell\IPersistFolder.htm
tech.root: shell
ms.assetid: d37d4ca5-93a0-4090-b657-9b23d5df875c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IPersistFolder, IPersistFolder interface [Windows Shell], IPersistFolder interface [Windows Shell],described, _win32_IPersistFolder, _win32_IPersistFolder_cpp, shell.IPersistFolder, shobjidl_core/IPersistFolder
ms.topic: interface
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Shell32.dll (version 4.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Shell32.dll
api_name:
 - IPersistFolder
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPersistFolder interface


## -description


Exposes a method that initializes Shell folder objects.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IPersistFolder</b> interface inherits from <a href="https://msdn.microsoft.com/932eb0e2-35a6-482e-9138-00cff30508a9">IPersist</a>. <b>IPersistFolder</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IPersistFolder</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/179f13c9-7306-4ed5-935e-2620616b46c1">Initialize</a>
</td>
<td align="left" width="63%">
Instructs a Shell folder object to initialize itself based on the information passed.

</td>
</tr>
</table> 


## -remarks



When you implement a Shell namespace extension, specifically the <a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a> interface, you must implement this interface so the folder object can be initialized. Implementation of this interface is how the folder is told where it is in the Shell namespace.

You do not use this interface directly. It is used by the file system implementation of the <a href="https://msdn.microsoft.com/5e699494-1974-4b9b-8324-9394f7b96fe4">IShellFolder::BindToObject</a> interface when it is initializing a Shell folder object.



