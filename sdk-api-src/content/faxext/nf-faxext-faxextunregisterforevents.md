---
UID: NF:faxext.FaxExtUnregisterForEvents
title: FaxExtUnregisterForEvents function
author: windows-sdk-content
description: The FaxExtUnregisterForEvents callback function unregisters the fax extension DLL for notifications about configuration data changes related to a specific device and GUID.
old-location: fax\_mfax_faxextunregisterforevents.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxextconfigref_7soj.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FaxExtUnregisterForEvents, FaxExtUnregisterForEvents function [Fax Service], _mfax_faxextunregisterforevents, fax._mfax_faxextunregisterforevents, faxext/FaxExtUnregisterForEvents
ms.topic: function
req.header: faxext.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - FaxExt.h
api_name:
 - FaxExtUnregisterForEvents
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FaxExtUnregisterForEvents function


## -description


The <b>FaxExtUnregisterForEvents</b> callback function unregisters the fax extension DLL for notifications about configuration data changes related to a specific device and GUID.


## -parameters




### -param hNotification

Type: <b>HANDLE</b>

Specifies a <b>HANDLE</b> that indicates the registration handle from which the caller wishes to unregister.




The handle must be the return value from a previous call to the <a href="https://msdn.microsoft.com/en-us/library/ms684532(v=VS.85).aspx">FaxExtRegisterForEvents</a> function.


## -returns



Type: <b>DWORD</b>

If the function succeeds, the return value is <b>ERROR_SUCCESS</b>.





If the function fails, the return value is a nonzero error code defined in WinError.h. You can call the Win32 <b>FormatMessage</b> function specifying the FORMAT_MESSAGE_FROM_SYSTEM flag to retrieve a generic description of the error.





The <b>FaxExtUnregisterForEvents</b> function can return the following error codes.


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
The unregistration process succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The registration handle specified by the hNotification parameter was not found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The <i>hNotification</i> parameter is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
Not enough memory is available to complete the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_GEN_FAILURE</b></dt>
</dl>
</td>
<td width="60%">
An internal failure at the fax server prevents access to the data.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SHUTDOWN_IN_PROGRESS</b></dt>
</dl>
</td>
<td width="60%">
The server is shutting down.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_BUSY</b></dt>
</dl>
</td>
<td width="60%">
The server cannot process a request for notifications while it is sending a notification about a data change. You should try calling the function at a later time.

</td>
</tr>
</table>
 




## -remarks



When the fax extension calls this fax service callback function, it must use the function pointer exposed by the fax service when the service calls the <a href="https://msdn.microsoft.com/en-us/library/ms684525(v=VS.85).aspx">FaxExtInitializeConfig</a> function.

The fax extension can call the <b>FaxExtUnregisterForEvents</b> function to stop receiving notifications about device configuration data changes. An extension registers for notifications by calling the fax service's callback function <a href="https://msdn.microsoft.com/en-us/library/ms684532(v=VS.85).aspx">FaxExtRegisterForEvents</a>.

The fax service passes a pointer to the <b>FaxExtUnregisterForEvents</b> callback function when the fax service calls the <a href="https://msdn.microsoft.com/en-us/library/ms684525(v=VS.85).aspx">FaxExtInitializeConfig</a> function. The PFAX_EXT_UNREGISTER_FOR_EVENTS data type is a pointer to a <b>FaxExtUnregisterForEvents</b> function.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms684525(v=VS.85).aspx">FaxExtInitializeConfig</a>



<a href="https://msdn.microsoft.com/en-us/library/ms684532(v=VS.85).aspx">FaxExtRegisterForEvents</a>
 

 

