---
UID: NF:imapi2.IMultisession.get_InUse
title: IMultisession::get_InUse (imapi2.h)
author: windows-sdk-content
description: Determines if this multi-session interface is the one you should use on the current media.
old-location: imapi\imultisession_get_inuse.htm
tech.root: imapi
ms.assetid: 35ebf336-0d67-422c-b6f7-2fd6ee3e7226
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMultisession interface [IMAPI],get_InUse method, IMultisession.get_InUse, IMultisession::get_InUse, get_InUse, get_InUse method [IMAPI], get_InUse method [IMAPI],IMultisession interface, imapi.imultisession_get_inuse, imapi2/IMultisession::get_InUse
ms.topic: method
req.header: imapi2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2.idl
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
 - imapi2.h
api_name:
 - IMultisession.get_InUse
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMultisession::get_InUse


## -description


Determines if this multi-session interface is the one you should use on the current media.


## -parameters




### -param value [out]

Is VARIANT_TRUE if this multi-session interface is the one you should use to write to the  current media. Otherwise, VARIANT_FALSE.


## -returns



S_OK is returned on success, but other success codes may be returned as a result of implementation. The following error codes are commonly returned on operation failure, but do not represent the only possible error values:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
Pointer is not valid.

Value: 0x80004003

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/a983af02-ee0e-4a62-8ae0-fb9a1e0c2571">IMultisession</a>



<a href="https://msdn.microsoft.com/d4eef9de-8b7e-4326-b66f-dddbe2b8a05d">IMultisession::put_InUse</a>
 

 

