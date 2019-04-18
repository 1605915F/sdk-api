---
UID: NF:winfax.FaxConnectFaxServerW
title: FaxConnectFaxServerW function (winfax.h)
author: windows-sdk-content
description: The FaxConnectFaxServer function connects a fax client application to the local fax server. The function returns a fax server handle that is required to call other fax client functions that facilitate job, device, configuration, and document management.
old-location: fax\_mfax_faxconnectfaxserver.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_3qya.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FaxConnectFaxServer, FaxConnectFaxServer function [Fax Service], FaxConnectFaxServerA, FaxConnectFaxServerW, _mfax_faxconnectfaxserver, fax._mfax_faxconnectfaxserver, winfax/FaxConnectFaxServer, winfax/FaxConnectFaxServerA, winfax/FaxConnectFaxServerW
ms.topic: function
req.header: winfax.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: FaxConnectFaxServerW (Unicode) and FaxConnectFaxServerA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WinFax.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - WinFax.lib
 - WinFax.dll
api_name:
 - FaxConnectFaxServer
 - FaxConnectFaxServerA
 - FaxConnectFaxServerW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# FaxConnectFaxServerW function


## -description


The <b>FaxConnectFaxServer</b> function connects a fax client application to the local fax server. The function returns a fax server handle that is required to call other fax client functions that facilitate job, device, configuration, and document management.


## -parameters




### -param MachineName [in, optional]

Type: <b>LPCTSTR</b>

This pointer must be <b>NULL</b> (an empty string), so that the application connects to the fax server on the local computer.


### -param FaxHandle [out]

Type: <b>LPHANDLE</b>

Pointer to a variable that receives a fax server handle that is required on subsequent calls to other fax client functions. If the fax server returns a null handle, it indicates an error.


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. GetLastError can return one of the following errors.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The <i>FaxHandle</i> parameter is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
An error occurred during memory allocation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The user under whose account the call was made does not have sufficient rights to the fax server.

</td>
</tr>
</table>
 




## -remarks



This function can only be used only with a local server. Use of a remote server is enabled in the <a href="https://msdn.microsoft.com/en-us/library/ms684513(v=VS.85).aspx">Fax Service Extended COM API</a>. For more information see the <a href="https://msdn.microsoft.com/en-us/library/ms692315(v=VS.85).aspx">IFaxServer::Connect</a> method.

A fax client application must call the <b>FaxConnectFaxServer</b> function successfully before it calls any other fax client function.

The fax client application must call the <a href="https://msdn.microsoft.com/en-us/library/ms691909(v=VS.85).aspx">FaxClose</a> function to disconnect from the fax server and deallocate the handle that the <b>FaxConnectFaxServer</b> function returns. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms692919(v=VS.85).aspx">Connecting to the Fax Server</a> and <a href="https://msdn.microsoft.com/en-us/library/ms690866(v=VS.85).aspx">Disconnecting from a Fax Server</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691947(v=VS.85).aspx">Fax Service Client API Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691909(v=VS.85).aspx">FaxClose</a>
 

 

