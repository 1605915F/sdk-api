---
UID: NF:vss.IVssAsync.Cancel
title: IVssAsync::Cancel (vss.h)
author: windows-sdk-content
description: The Cancel method cancels an incomplete asynchronous operation.
old-location: base\ivssasync_cancel.htm
tech.root: VSS
ms.assetid: 8ab44737-114b-4edc-a097-d0fa297f6276
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Cancel, Cancel method [VSS], Cancel method [VSS],IVssAsync interface, IVssAsync interface [VSS],Cancel method, IVssAsync.Cancel, IVssAsync::Cancel, _win32_ivssasync_cancel, base.ivssasync_cancel, vss/IVssAsync::Cancel
ms.topic: method
req.header: vss.h
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
req.lib: VssApi.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - VssApi.lib
 - VssApi.dll
api_name:
 - IVssAsync.Cancel
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVssAsync::Cancel


## -description


The 
<b>Cancel</b> method cancels an incomplete asynchronous operation.


## -parameters






## -returns



All calls to 
<b>Cancel</b> for all 
<a href="https://msdn.microsoft.com/d2cff547-b4ff-454d-8e0e-cd29b91cbb07">IVssAsync</a> objects support the following status codes.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The asynchronous operation had been successfully canceled.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VSS_S_ASYNC_CANCELLED</b></dt>
</dl>
</td>
<td width="60%">
The asynchronous operation had been canceled prior to calling this method.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VSS_S_ASYNC_FINISHED</b></dt>
</dl>
</td>
<td width="60%">
The asynchronous operation had completed prior to calling this method.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VSS_E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
Unexpected error. The error code is logged in the error log file. For more information, see 
        <a href="https://msdn.microsoft.com/6377d937-5739-45f5-9195-5d18be4069ce">Event and Error Handling Under VSS</a>.

<b>Windows Server 2008, Windows Vista, Windows Server 2003 and Windows XP:  </b>This value is not supported until Windows Server 2008 R2 and Windows 7. E_UNEXPECTED is used instead.

</td>
</tr>
</table>
 

If an operation has completed unsuccessfully before 
<b>Cancel</b> was called, then 
<b>Cancel</b> returns the error that operation encountered.

To obtain a complete list of return values for a specific <b>IVssAsync::Cancel</b>, see the error codes of the method that returned the 
<a href="https://msdn.microsoft.com/d2cff547-b4ff-454d-8e0e-cd29b91cbb07">IVssAsync</a> object.




## -see-also




<a href="https://msdn.microsoft.com/d2cff547-b4ff-454d-8e0e-cd29b91cbb07">IVssAsync</a>



<a href="https://msdn.microsoft.com/85fb3ae8-dc09-4f6f-a96b-e4dc046ff48a">IVssAsync::QueryStatus</a>
 

 

