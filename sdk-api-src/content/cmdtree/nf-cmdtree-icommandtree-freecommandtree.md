---
UID: NF:cmdtree.ICommandTree.FreeCommandTree
title: ICommandTree::FreeCommandTree
author: windows-sdk-content
description: The ICommandTree::FreeCommandTree method traverses a command tree and deallocates all DBCOMMANDTREE node structures, as well as all variants in those structures. It then sets the root pointer to a NULL pointer.
old-location: indexsrv\icommandtree_freecommandtree.htm
tech.root: IndexSrv
ms.assetid: VS|indexsrv|~\html\ixoledb_1v39.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FreeCommandTree, FreeCommandTree method [Indexing Service], FreeCommandTree method [Indexing Service],ICommandTree interface, ICommandTree interface [Indexing Service],FreeCommandTree method, ICommandTree.FreeCommandTree, ICommandTree::FreeCommandTree, _idxs_ICommandTree_FreeCommandTree, cmdtree/ICommandTree::FreeCommandTree, indexsrv.icommandtree_freecommandtree
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: cmdtree.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: CmdTre.idl
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
 - cmdtree.h
api_name:
 - ICommandTree.FreeCommandTree
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICommandTree::FreeCommandTree


## -description


<p class="CCE_Message">[Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use <a href="https://msdn.microsoft.com/en-us/library/Aa965362(v=VS.85).aspx">Windows Search</a> for client side search and  <a href=" http://go.microsoft.com/fwlink/p/?linkid=258445">Microsoft Search Server Express</a> for server side search.]

The <b>ICommandTree::FreeCommandTree</b> method traverses a command tree and deallocates all <a href="https://msdn.microsoft.com/en-us/library/ms689889(v=VS.85).aspx">DBCOMMANDTREE</a> node structures, as well as all variants in those structures. It then sets the root pointer to a <b>NULL</b> pointer.


## -parameters




### -param ppRoot [in]

Pointer to a variable that receives the pointer to the root of the command tree on successful exit.


## -returns



This method can return one of these values.

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
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
A provider-specific error occurred.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppRoot</i> parameter was a <b>NULL</b> pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DB_E_CANNOTFREE</b></dt>
</dl>
</td>
<td width="60%">
The consumer called the <a href="https://msdn.microsoft.com/en-us/library/ms690251(v=VS.85).aspx">ICommandTree::SetCommandTree</a> method with <i>fCopy</i> = <b>FALSE</b>, thereby relinquishing ownership of the memory to the provider.

</td>
</tr>
</table>
 




## -remarks



The <b>FreeCommandTree</b> method can be used by a consumer to free its copy of the command tree constructed locally or obtained by <a href="https://msdn.microsoft.com/en-us/library/ms689887(v=VS.85).aspx">ICommandTree::GetCommandTree</a>. It does not free the copy of the tree owned by the command object. When a consumer calls <a href="https://msdn.microsoft.com/en-us/library/ms690251(v=VS.85).aspx">SetCommandTree</a> with <i>fCopy</i> = <b>FALSE</b>, the consumer relinquishes ownership of the memory to the provider. Therefore, if the consumer calls <b>FreeCommandTree</b> after having called <b>SetCommandTree</b> with <i>fCopy</i> = <b>FALSE</b>, <b>FreeCommandTree</b> returns a DB_E_CANNOTFREE error code, meaning the consumer does not have ownership of the tree and is unable to free it.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms689746(v=VS.85).aspx">ICommandTree</a>
 

 

