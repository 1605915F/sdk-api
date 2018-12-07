---
UID: NF:netioapi.ConvertInterfaceLuidToAlias
title: ConvertInterfaceLuidToAlias function
author: windows-sdk-content
description: Converts a locally unique identifier (LUID) for a network interface to an interface alias.
old-location: iphlp\convertinterfaceluidtoalias.htm
tech.root: IpHlp
ms.assetid: 86a821c1-e04b-4bc3-846d-767c55008aed
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ConvertInterfaceLuidToAlias, ConvertInterfaceLuidToAlias function [IP Helper], iphlp.convertinterfaceluidtoalias, netioapi/ConvertInterfaceLuidToAlias
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: netioapi.h
req.include-header: Iphlpapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Iphlpapi.lib
req.dll: Iphlpapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Iphlpapi.dll
api_name:
 - ConvertInterfaceLuidToAlias
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ConvertInterfaceLuidToAlias function


## -description


The 
<b>ConvertInterfaceLuidToAlias</b> function converts a locally unique identifier (LUID) for a network interface to an interface alias.


## -parameters




### -param InterfaceLuid [in]

A pointer to a <a href="https://msdn.microsoft.com/c4956c5a-3c6c-4f1c-b9d7-2e377b66f197">NET_LUID</a> for a network interface.


### -param InterfaceAlias [out]

A pointer to a buffer to hold the <b>NULL</b>-terminated Unicode string containing the alias name of the network interface when the function returns successfully.


### -param Length [in]

The length, in characters, of the buffer pointed to by the <i>InterfaceAlias</i> parameter. This value must be large enough to accommodate the alias name of the network interface and the terminating <b>NULL</b> character.  The maximum required length is
        <b>NDIS_IF_MAX_STRING_SIZE</b> + 1.


## -returns



On success, 
<b>ConvertInterfaceLuidToAlias</b> returns NO_ERROR. Any nonzero return value indicates failure. 

<table>
<tr>
<th>Error code</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One of the parameters was invalid. This error is returned if either the <i>InterfaceLuid</i> or <i>InterfaceAlias</i> parameter was <b>NULL</b> or if the <i>InterfaceLuid</i> parameter was invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
Not enough storage is available to process this command. This error is returned if the size of the buffer pointed to by the <i>InterfaceAlias</i> parameter was not large enough as specified in the <i>Length</i> parameter to hold the alias name.

</td>
</tr>
</table>
 




## -remarks



The <b>ConvertInterfaceLuidToAlias</b> function is available on Windows Vistaand later.

The <b>ConvertInterfaceLuidToAlias</b> function is protocol independent and works with network interfaces for both the IPv6 and IPv4 protocol.

The maximum length of the alias name for a network interface, <b>NDIS_IF_MAX_STRING_SIZE</b>, without the terminating <b>NULL</b> is declared in the <i>Ntddndis.h</i> header file. The <b>NDIS_IF_MAX_STRING_SIZE</b> is defined to be the <b>IF_MAX_STRING_SIZE</b> constant defined in the <i>Ifdef.h</i> header file. The <i>Ntddndis.h</i> and <i>Ifdef.h</i> header files are automatically included in the <i>Netioapi.h</i> header file which is automatically included by the <i>Iphlpapi.h</i> header file. The <i>Ntddndis.h</i>, <i>Ifdef.h</i>, and <i> Netioapi.h</i> header files should never be used directly. 





## -see-also




<a href="https://msdn.microsoft.com/7fa80938-d475-4ace-b463-a53aac26e88b">ConvertInterfaceAliasToLuid</a>



<a href="https://msdn.microsoft.com/cae669dc-899b-4485-b70a-5f58207a07df">ConvertInterfaceGuidToLuid</a>



<a href="https://msdn.microsoft.com/c757228c-93f1-4545-8921-9d048bca580c">ConvertInterfaceIndexToLuid</a>



<a href="https://msdn.microsoft.com/9d5bd1e9-0bf1-405a-8726-8e2c9ba4e022">ConvertInterfaceLuidToGuid</a>



<a href="https://msdn.microsoft.com/904cd94c-dd46-42ac-aef2-ffed4b3e5899">ConvertInterfaceLuidToIndex</a>



<a href="https://msdn.microsoft.com/c65f7b3c-55f4-40f8-9a7a-19d1066deca4">ConvertInterfaceLuidToNameA</a>



<a href="https://msdn.microsoft.com/e4269a6a-1237-4503-b7d7-756388458750">ConvertInterfaceLuidToNameW</a>



<a href="https://msdn.microsoft.com/daceabf9-ff43-4206-9f8f-f3924de9c5a5">ConvertInterfaceNameToLuidA</a>



<a href="https://msdn.microsoft.com/473be9f0-7fac-46f0-b33c-839906411fdc">ConvertInterfaceNameToLuidW</a>



<a href="https://msdn.microsoft.com/c4956c5a-3c6c-4f1c-b9d7-2e377b66f197">NET_LUID</a>



<a href="https://msdn.microsoft.com/0da31819-3ee7-4474-9e68-f5a18d4a135a">if_indextoname</a>



<a href="https://msdn.microsoft.com/599e5a34-1e17-4c5f-b58e-727871e409be">if_nametoindex</a>
 

 

