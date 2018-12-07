---
UID: NF:bits3_0.IBitsPeerCacheAdministration.DeleteUrl
title: IBitsPeerCacheAdministration::DeleteUrl
author: windows-sdk-content
description: Deletes all cache records and the file from the cache for the given URL.
old-location: bits\ibitspeercacheadministration_deleteurl.htm
tech.root: bits
ms.assetid: d4849830-62fa-4bf4-bfad-59bcdbf1a10e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DeleteUrl, DeleteUrl method [BITS], DeleteUrl method [BITS],IBitsPeerCacheAdministration interface, IBitsPeerCacheAdministration interface [BITS],DeleteUrl method, IBitsPeerCacheAdministration.DeleteUrl, IBitsPeerCacheAdministration::DeleteUrl, bits.ibitspeercacheadministration_deleteurl, bits3_0/IBitsPeerCacheAdministration::DeleteUrl
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: bits3_0.h
req.include-header: Bits.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits3_0.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Bits.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Bits.lib
 - Bits.dll
api_name:
 - IBitsPeerCacheAdministration.DeleteUrl
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBitsPeerCacheAdministration::DeleteUrl


## -description


Deletes all cache records and the file from the cache for the given URL. 


## -parameters




### -param url [in]

Null-terminated string that contains the URL of the file whose cache records and file you want to delete from the cache. 


## -returns



The method returns the following return values.

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
Success

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The URL does not exist.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>BG_E_BUSYCACHERECORD</b></dt>
</dl>
</td>
<td width="60%">
The cache record is in use and cannot be changed or deleted.  Try again after a few seconds.

</td>
</tr>
</table>
 




## -remarks



The cache records for the file are not removed until all current activity with the cache records is complete.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa964272(v=VS.85).aspx">IBitsPeerCacheAdministration</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa964275(v=VS.85).aspx">IBitsPeerCacheAdministration::DeleteRecord</a>
 

 

