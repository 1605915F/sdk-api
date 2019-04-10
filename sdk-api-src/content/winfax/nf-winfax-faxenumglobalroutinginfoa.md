---
UID: NF:winfax.FaxEnumGlobalRoutingInfoA
title: FaxEnumGlobalRoutingInfoA function (winfax.h)
author: windows-sdk-content
description: The FaxEnumGlobalRoutingInfo function enumerates all fax routing methods associated with a specific fax server.
old-location: fax\_mfax_faxenumglobalroutinginfo.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_5zvz.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FaxEnumGlobalRoutingInfo, FaxEnumGlobalRoutingInfo function [Fax Service], FaxEnumGlobalRoutingInfoA, FaxEnumGlobalRoutingInfoW, _mfax_faxenumglobalroutinginfo, fax._mfax_faxenumglobalroutinginfo, winfax/FaxEnumGlobalRoutingInfo, winfax/FaxEnumGlobalRoutingInfoA, winfax/FaxEnumGlobalRoutingInfoW
ms.topic: function
req.header: winfax.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: FaxEnumGlobalRoutingInfoW (Unicode) and FaxEnumGlobalRoutingInfoA (ANSI)
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
 - FaxEnumGlobalRoutingInfo
 - FaxEnumGlobalRoutingInfoA
 - FaxEnumGlobalRoutingInfoW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FaxEnumGlobalRoutingInfoA function


## -description


The <b>FaxEnumGlobalRoutingInfo</b> function enumerates all fax routing methods associated with a specific fax server. The function returns to the fax client application fax routing method information that applies globally to the server, such as routing priority.


## -parameters




### -param FaxHandle [in]

Type: <b>HANDLE</b>

Specifies a fax server handle returned by a call to the <a href="https://msdn.microsoft.com/en-us/library/ms691482(v=VS.85).aspx">FaxConnectFaxServer</a> function.


### -param RoutingInfo [out]

Type: <b>PFAX_GLOBAL_ROUTING_INFO*</b>

Pointer to the address of a buffer to receive an array of <a href="https://msdn.microsoft.com/en-us/library/ms690746(v=VS.85).aspx">FAX_GLOBAL_ROUTING_INFO</a> structures. Each structure contains information about one fax routing method, as it pertains to the entire fax service. The data includes, among other items, the priority for the fax routing method, and the name of the DLL that exports the routing method. It also includes the GUID and function name that identify the routing method, and the method's user-friendly name. For information about memory allocation, see the following Remarks section.


### -param MethodsReturned [out]

Type: <b>LPDWORD</b>

Pointer to a DWORD variable to receive the number of <a href="https://msdn.microsoft.com/en-us/library/ms690746(v=VS.85).aspx">FAX_GLOBAL_ROUTING_INFO</a> structures the function returns in the <i>RoutingInfo</i> parameter. This number equals the total number of fax routing methods installed on the target server.


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
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
Access is denied. <a href="https://msdn.microsoft.com/en-us/library/ms692302(v=VS.85).aspx">FAX_CONFIG_QUERY</a> access is required.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One or all of the <i>MethodsReturned</i>, <i>RoutingInfo</i> or <i>FaxHandle</i> parameters are <b>NULL</b>.

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
</table>
 




## -remarks



The <b>FaxEnumGlobalRoutingInfo</b> function retrieves fax routing method information, such as routing priority, that applies globally to the fax server. An application can modify global data by calling the <a href="https://msdn.microsoft.com/en-us/library/ms691451(v=VS.85).aspx">FaxSetGlobalRoutingInfo</a> function.

An application can call the <a href="https://msdn.microsoft.com/en-us/library/ms691804(v=VS.85).aspx">FaxEnumRoutingMethods</a> function to enumerate the fax routing methods associated with a particular device.

The <b>FaxEnumGlobalRoutingInfo</b> function allocates the memory required for the <a href="https://msdn.microsoft.com/en-us/library/ms690746(v=VS.85).aspx">FAX_GLOBAL_ROUTING_INFO</a> buffer array pointed to by the <i>RoutingInfo</i> parameter. An application must call the <a href="https://msdn.microsoft.com/en-us/library/ms692846(v=VS.85).aspx">FaxFreeBuffer</a> function to deallocate the resources associated with this parameter. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms690878(v=VS.85).aspx">Freeing Fax Resources</a> and <a href="https://msdn.microsoft.com/en-us/library/ms691940(v=VS.85).aspx">Managing Fax Routing Data</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms690746(v=VS.85).aspx">FAX_GLOBAL_ROUTING_INFO</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691947(v=VS.85).aspx">Fax Service Client API Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691482(v=VS.85).aspx">FaxConnectFaxServer</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691804(v=VS.85).aspx">FaxEnumRoutingMethods</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692846(v=VS.85).aspx">FaxFreeBuffer</a>



<a href="https://msdn.microsoft.com/en-us/library/ms691451(v=VS.85).aspx">FaxSetGlobalRoutingInfo</a>
 

 

