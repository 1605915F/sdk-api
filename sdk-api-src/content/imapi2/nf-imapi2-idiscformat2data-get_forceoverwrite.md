---
UID: NF:imapi2.IDiscFormat2Data.get_ForceOverwrite
title: IDiscFormat2Data::get_ForceOverwrite
author: windows-sdk-content
description: Determines if the data writer must overwrite the disc on overwritable media types.
old-location: imapi\idiscformat2data_get_forceoverwrite.htm
tech.root: imapi
ms.assetid: ac1bfca7-e681-4e88-85d6-c77ffcbe7872
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDiscFormat2Data interface [IMAPI],get_ForceOverwrite method, IDiscFormat2Data.get_ForceOverwrite, IDiscFormat2Data::get_ForceOverwrite, get_ForceOverwrite, get_ForceOverwrite method [IMAPI], get_ForceOverwrite method [IMAPI],IDiscFormat2Data interface, imapi.idiscformat2data_get_forceoverwrite, imapi2/IDiscFormat2Data::get_ForceOverwrite
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
 - IDiscFormat2Data.get_ForceOverwrite
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDiscFormat2Data::get_ForceOverwrite


## -description


Determines if the data writer must overwrite the disc on overwritable media types.


## -parameters




### -param value [out]

Is VARIANT_TRUE if the data writer must overwrite the disc on overwritable media types; otherwise, VARIANT_FALSE.


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




<a href="https://msdn.microsoft.com/6bb871c2-1a6e-4cf6-94e1-7a566ce7a88e">IDiscFormat2Data</a>
 

 

