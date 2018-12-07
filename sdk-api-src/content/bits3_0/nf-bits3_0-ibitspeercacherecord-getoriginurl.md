---
UID: NF:bits3_0.IBitsPeerCacheRecord.GetOriginUrl
title: IBitsPeerCacheRecord::GetOriginUrl
author: windows-sdk-content
description: Gets the origin URL of the cached file.
old-location: bits\ibitspeercacherecord_getoriginurl.htm
tech.root: bits
ms.assetid: 9d74df3a-89e0-4a3a-82f3-c2e79c609b21
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetOriginUrl, GetOriginUrl method [BITS], GetOriginUrl method [BITS],IBitsPeerCacheRecord interface, IBitsPeerCacheRecord interface [BITS],GetOriginUrl method, IBitsPeerCacheRecord.GetOriginUrl, IBitsPeerCacheRecord::GetOriginUrl, bits.ibitspeercacherecord_getoriginurl, bits3_0/IBitsPeerCacheRecord::GetOriginUrl
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
 - IBitsPeerCacheRecord.GetOriginUrl
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBitsPeerCacheRecord::GetOriginUrl


## -description


Gets the origin URL of the cached file.


## -parameters




### -param pVal [in]

Null-terminated string that contains the origin URL of the cached file. Call the 
<a href="https://msdn.microsoft.com/en-us/library/ms680722(v=VS.85).aspx">CoTaskMemFree</a> function to free <i>ppOriginUrl</i> when done.


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



This URL may be different than the URL originally specified in the BITS job if <a href="https://msdn.microsoft.com/en-us/library/Aa964260(v=VS.85).aspx">IBackgroundCopyJobHttpOptions::SetSecurityFlags</a> is set to BG_HTTP_REDIRECT_POLICY_ALLOW_REPORT or BG_HTTP_REDIRECT_POLICY_DISALLOW.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa964291(v=VS.85).aspx">IBitsPeerCacheRecord</a>
 

 

