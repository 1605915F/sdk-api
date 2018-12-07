---
UID: NF:cscobj.IOfflineFilesCache.IsPathCacheable
title: IOfflineFilesCache::IsPathCacheable
author: windows-sdk-content
description: Determines whether a specified UNC path is in the Offline Files cache.
old-location: of\iofflinefilescache_ispathcacheable.htm
tech.root: offlinefiles
ms.assetid: 4d9a2fda-baad-4ada-8a07-f39c9cfafdfa
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: IOfflineFilesCache interface [Offline Files],IsPathCacheable method, IOfflineFilesCache.IsPathCacheable, IOfflineFilesCache::IsPathCacheable, IsPathCacheable, IsPathCacheable method [Offline Files], IsPathCacheable method [Offline Files],IOfflineFilesCache interface, OFFLINEFILES_CACHING_MODE_AUTO_DOC, OFFLINEFILES_CACHING_MODE_AUTO_PROGANDDOC, OFFLINEFILES_CACHING_MODE_MANUAL, OFFLINEFILES_CACHING_MODE_NOCACHING, OFFLINEFILES_CACHING_MODE_NONE, cscobj/IOfflineFilesCache::IsPathCacheable, of.iofflinefilescache_ispathcacheable
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: CscSvc.dll; CscObj.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CscSvc.dll
 - CscObj.dll
api_name:
 - IOfflineFilesCache.IsPathCacheable
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOfflineFilesCache::IsPathCacheable


## -description


Determines whether a specified UNC path is in the Offline Files cache.


## -parameters




### -param pszPath [in]

The UNC path of the item.


### -param pbCacheable [out]

Receives <b>TRUE</b> if the item is in the Offline Files cache, <b>FALSE</b> if not.


### -param pShareCachingMode [out]

Receives one of the following <a href="https://msdn.microsoft.com/en-us/library/Bb530642(v=VS.85).aspx">OFFLINEFILES_CACHING_MODE</a> enumeration values indicating the caching configuration of the applicable network shared folder under which the specified item exists.



#### OFFLINEFILES_CACHING_MODE_NONE (0)

No caching mode value was found.  This value is used when the item is not cacheable or an error has occurred.



#### OFFLINEFILES_CACHING_MODE_NOCACHING (1)

The shared folder is configured to disallow caching.



#### OFFLINEFILES_CACHING_MODE_MANUAL (2)

The shared folder is configured to allow manual caching.



#### OFFLINEFILES_CACHING_MODE_AUTO_DOC (3)

The shared folder is configured to allow automatic caching of documents.



#### OFFLINEFILES_CACHING_MODE_AUTO_PROGANDDOC (4)

The shared folder is configured to allow automatic caching of programs and documents.


## -returns



Returns <b>S_OK</b> if successful, or an error value otherwise.




## -remarks



The caching mode value returned is equivalent to the <b>CSC_MASK</b> value associated with <a href="https://msdn.microsoft.com/en-us/library/Bb525404(v=VS.85).aspx">SHARE_INFO_1005</a> returned by <a href="https://msdn.microsoft.com/en-us/library/Bb525388(v=VS.85).aspx">NetShareGetInfo</a>.  The value mapping is as follows:

<table>
<tr>
<th>
<a href="https://msdn.microsoft.com/en-us/library/Bb530642(v=VS.85).aspx">OFFLINEFILES_CACHING_MODE</a> Value</th>
<th>
<a href="https://msdn.microsoft.com/en-us/library/Bb525404(v=VS.85).aspx">SHARE_INFO_1005</a> Value</th>
</tr>
<tr>
<td><b>OFFLINEFILES_CACHING_MODE_NOCACHING</b></td>
<td>0</td>
</tr>
<tr>
<td><b>OFFLINEFILES_CACHING_MODE_MANUAL</b></td>
<td><b>CSC_CACHE_MANUAL_REINT</b></td>
</tr>
<tr>
<td><b>OFFLINEFILES_CACHING_MODE_AUTO_DOC</b></td>
<td><b>CSC_CACHE_AUTO_REINT</b></td>
</tr>
<tr>
<td><b>OFFLINEFILES_CACHING_MODE_AUTO_PROGANDDOC</b></td>
<td><b>CSC_CACHE_VDO</b></td>
</tr>
</table>
 

These settings are configured as attributes of the shared folder on the server by clicking the Caching button on the shared folder's Sharing property page or by using the <code>net share /cache</code> command.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb530486(v=VS.85).aspx">IOfflineFilesCache</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb530612(v=VS.85).aspx">IOfflineFilesShareInfo::GetShareCachingMode</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb530642(v=VS.85).aspx">OFFLINEFILES_CACHING_MODE</a>
 

 

