---
UID: NF:bits3_0.IBitsPeerCacheAdministration.GetMaximumCacheSize
title: IBitsPeerCacheAdministration::GetMaximumCacheSize
author: windows-sdk-content
description: Gets the maximum size of the cache.
old-location: bits\ibitspeercacheadministration_getmaximumcachesize.htm
tech.root: bits
ms.assetid: 6ea0e6f7-c674-4088-9085-5f6246681009
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetMaximumCacheSize, GetMaximumCacheSize method [BITS], GetMaximumCacheSize method [BITS],IBitsPeerCacheAdministration interface, IBitsPeerCacheAdministration interface [BITS],GetMaximumCacheSize method, IBitsPeerCacheAdministration.GetMaximumCacheSize, IBitsPeerCacheAdministration::GetMaximumCacheSize, bits.ibitspeercacheadministration_getmaximumcachesize, bits3_0/IBitsPeerCacheAdministration::GetMaximumCacheSize
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
 - IBitsPeerCacheAdministration.GetMaximumCacheSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBitsPeerCacheAdministration::GetMaximumCacheSize


## -description


Gets the maximum size of the cache.


## -parameters




### -param pBytes [out]

Maximum size of the cache, as a percentage of available hard disk drive space.


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
 




## -see-also




<a href="https://msdn.microsoft.com/5fa30b4e-f13c-4341-af65-a2e3d2703b96">IBitsPeerCacheAdministration</a>



<a href="https://msdn.microsoft.com/064376cf-8865-45a1-a63a-1096bc0d58ce">IBitsPeerCacheAdministration::SetMaximumCacheSize</a>
 

 

