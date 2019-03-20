---
UID: NF:bits3_0.IBitsPeerCacheAdministration.ClearRecords
title: IBitsPeerCacheAdministration::ClearRecords (bits3_0.h)
author: windows-sdk-content
description: Removes all the records and files from the cache.
old-location: bits\ibitspeercacheadministration_clearrecords.htm
tech.root: Bits
ms.assetid: 96e18c5d-6c76-4953-8e8e-3e98943478d8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClearRecords, ClearRecords method [BITS], ClearRecords method [BITS],IBitsPeerCacheAdministration interface, IBitsPeerCacheAdministration interface [BITS],ClearRecords method, IBitsPeerCacheAdministration.ClearRecords, IBitsPeerCacheAdministration::ClearRecords, bits.ibitspeercacheadministration_clearrecords, bits3_0/IBitsPeerCacheAdministration::ClearRecords
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
 - IBitsPeerCacheAdministration.ClearRecords
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBitsPeerCacheAdministration::ClearRecords


## -description


Removes all the records and files from the cache.


## -parameters






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
</table>
 




## -remarks



The cache is not cleared until all current cache activity is complete.




## -see-also




<a href="https://msdn.microsoft.com/5fa30b4e-f13c-4341-af65-a2e3d2703b96">IBitsPeerCacheAdministration</a>



<a href="https://msdn.microsoft.com/c86199c3-9fe7-4d8f-8b33-b12b65b94e54">IBitsPeerCacheAdministration::DeleteRecord</a>
 

 

