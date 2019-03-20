---
UID: NS:shlobj_core.SHARDAPPIDINFO
title: SHARDAPPIDINFO (shlobj_core.h)
author: windows-sdk-content
description: Contains data used by SHAddToRecentDocs to identify both an item&#8212;in this case as an IShellItem&#8212;and the process that it is associated with.
old-location: shell\SHARDAPPIDINFO.htm
tech.root: shell
ms.assetid: bb2b7e86-04ca-4dd0-944b-a95e8a0be1e0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SHARDAPPIDINFO, SHARDAPPIDINFO structure [Windows Shell], _shell_SHARDAPPIDINFO, shell.SHARDAPPIDINFO, shlobj_core/SHARDAPPIDINFO
ms.topic: struct
req.header: shlobj_core.h
req.include-header: Shlobj.h
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
 - HeaderDef
api_location:
 - shlobj_core.h
api_name:
 - SHARDAPPIDINFO
product: Windows
targetos: Windows
req.typenames: SHARDAPPIDINFO
req.redist: 
---

# SHARDAPPIDINFO structure


## -description


Contains data used by <a href="https://msdn.microsoft.com/84e065e6-b68d-4303-b98b-3f8507539468">SHAddToRecentDocs</a> to identify both an item—in this case as an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>—and the process that it is associated with.


## -struct-fields




### -field psi

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>*</b>

Pointer to an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> object that represents the object in the Shell namespace.


### -field pszAppID

Type: <b>PCWSTR</b>

The application-defined AppUserModelID associated with the item.


## -see-also




<a href="https://msdn.microsoft.com/ebce2d99-6f20-4545-9f12-d79cd8d0828f">Application User Model IDs (AppUserModelIDs)</a>



<a href="https://msdn.microsoft.com/11c69ff9-b8a0-4168-8036-f45a9f7813ba">SHARDAPPIDINFOIDLIST</a>



<a href="https://msdn.microsoft.com/01613dc9-4516-4995-bd31-feee2eb650b2">SHARDAPPIDINFOLINK</a>



<a href="https://msdn.microsoft.com/84e065e6-b68d-4303-b98b-3f8507539468">SHAddToRecentDocs</a>
 

 

