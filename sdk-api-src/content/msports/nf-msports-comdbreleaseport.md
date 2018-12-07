---
UID: NF:msports.ComDBReleasePort
title: ComDBReleasePort function
author: windows-sdk-content
description: ComDBReleasePort releases a COM port number in the COM port database.
old-location: serports\comdbreleaseport.htm
tech.root: serports
ms.assetid: bece99c5-75de-4ab4-be26-14dc8cc1819c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ComDBReleasePort, ComDBReleasePort function [Serial Ports], comdb_dd9f4f27-aea1-4bd8-aa59-ca5aaa05e210.xml, msports/ComDBReleasePort, serports.comdbreleaseport
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: msports.h
req.include-header: Msports.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Msports.lib
req.dll: Msports.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Msports.dll
api_name:
 - ComDBReleasePort
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ComDBReleasePort function


## -description


<b>ComDBReleasePort</b> releases a COM port number in the COM port database.


## -parameters




### -param HComDB [in]

Handle to the COM port database that was returned by <a href="https://msdn.microsoft.com/6ae22de0-b71e-441d-af12-8518a3f474e3">ComDBOpen</a>.


### -param ComNumber [in]

Specifies the COM port number to release. A port number is an integer that ranges from one to COMDB_MAX_PORTS_ARBITRATED.


## -returns



<b>ComDBReleasePort</b> returns one of the following status values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
</dl>
</td>
<td width="60%">
The COM port number was released.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_CANTWRITE</b></dt>
</dl>
</td>
<td width="60%">
The routine could not write to the database.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One of the following is true: The specified handle to the COM port database is not valid. The specified port number is not in the COM port database.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_CONNECTED</b></dt>
</dl>
</td>
<td width="60%">
The routine could not access the database. To get extended error information, call <b>GetLastError</b>.

</td>
</tr>
</table>
 




## -remarks



<i>Releasing</i> a COM port number means to log the port number as "not in use".

<b>ComDBReleasePort</b> runs in user mode.

For more information, see <a href="https://msdn.microsoft.com/c9baf147-6e33-4ed2-b682-c141938eb0da">Obtaining and Releasing a COM Port Number</a>.




## -see-also




<a href="https://msdn.microsoft.com/b32b42e8-d38c-4bb5-bf8a-96538a03cb5b">ComDBClaimNextFreePort</a>



<a href="https://msdn.microsoft.com/d0baa783-1039-41a4-8bb1-78c977ed62b6">ComDBClaimPort</a>
 

 

