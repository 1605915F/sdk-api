---
UID: NF:dskquota.IDiskQuotaUser.SetQuotaLimit
title: IDiskQuotaUser::SetQuotaLimit
author: windows-sdk-content
description: Sets the user's quota limit value on the volume.
old-location: fs\idiskquotauser_setquotalimit.htm
tech.root: FileIO
ms.assetid: f7c99415-685b-4a21-ac7b-68f4816aafb0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDiskQuotaUser interface [Files],SetQuotaLimit method, IDiskQuotaUser.SetQuotaLimit, IDiskQuotaUser::SetQuotaLimit, SetQuotaLimit, SetQuotaLimit method [Files], SetQuotaLimit method [Files],IDiskQuotaUser interface, _win32_idiskquotauser_setquotalimit, base.idiskquotauser_setquotalimit, dskquota/IDiskQuotaUser::SetQuotaLimit, fs.idiskquotauser_setquotalimit
ms.topic: method
req.header: dskquota.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Dskquota.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dskquota.dll
api_name:
 - IDiskQuotaUser.SetQuotaLimit
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDiskQuotaUser::SetQuotaLimit


## -description


Sets the user's quota limit value on the volume. The limit is set as the maximum amount of disk space available to the volume user.


## -parameters




### -param llLimit [in]

The default quota limit, in bytes. If this value is -1, the user has an unlimited quota.


### -param fWriteThrough [in]

If this value is <b>TRUE</b>, the value is written immediately to the volume's quota file. Otherwise, the value is written only to the quota user object's local memory. This value should typically be set to <b>TRUE</b>. Set it to <b>FALSE</b> when using the 
<a href="https://msdn.microsoft.com/6cb3da5d-8e4c-45de-b9cf-0f6abf3f1932">IDiskQuotaUserBatch</a> interface to modify multiple user quota entries at once.


## -returns



This method returns a file system error or one of the following values.

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
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The caller has insufficient access rights.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_LOCK_FAILED</b></dt>
</dl>
</td>
<td width="60%">
Failure to obtain an exclusive lock.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unexpected file system error occurred.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/c1f79e2e-834b-41dc-a15f-6dd1034d021b">Disk Management Interfaces</a>



<a href="https://msdn.microsoft.com/42efbd5b-6455-4319-a76e-cdb666fc36b8">Disk Quotas</a>



<a href="https://msdn.microsoft.com/27edbebc-35b4-4f6a-87cc-d8a99782f405">IDiskQuotaUser</a>
 

 

