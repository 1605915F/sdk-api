---
UID: NF:rtmv2.RTM_IPV4_GET_ADDR_AND_LEN
title: RTM_IPV4_GET_ADDR_AND_LEN macro (rtmv2.h)
author: windows-sdk-content
description: The RTM_IPV4_GET_ADDR_AND_LEN macro converts a generic net address and length to an IPv4 RTM_NET_ADDRESS structure and length.
old-location: rras\rtm_ipv4_get_addr_and_len.htm
tech.root: RRAS
ms.assetid: e37bb309-845c-4685-bbfd-15ffc6c74fd0
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: RTM_IPV4_GET_ADDR_AND_LEN, RTM_IPV4_GET_ADDR_AND_LEN macro [RAS], _rtmv2ref_rtm_ipv4_get_addr_and_len, rras.rtm_ipv4_get_addr_and_len, rtmv2/RTM_IPV4_GET_ADDR_AND_LEN
ms.topic: macro
req.header: rtmv2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Rtmv2.h
api_name:
 - RTM_IPV4_GET_ADDR_AND_LEN
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# RTM_IPV4_GET_ADDR_AND_LEN macro


## -description


The 
<b>RTM_IPV4_GET_ADDR_AND_LEN</b> macro converts a generic net address and length to an IPv4 <a href="https://msdn.microsoft.com/92c4e797-9b73-438d-b4df-9739fae9d5c8">RTM_NET_ADDRESS</a> structure and length.


## -parameters




### -param Addr

Receives the converted IPv4 address.


### -param Len

Receives the converted length.


### -param NetAddress

Specifies the network address to convert.


## -remarks



For example, if a client supplies the <i>NetAddress</i> 10.10.10/24, the <i>Addr</i> 10.10.10.0 and the <i>Len</i> 24 are returned.

The macro is defined as follows:


```cpp
#include <windows.h>

#define RTM_IPV4_GET_ADDR_AND_LEN(Addr, Len, NetAddress)    \
        (Len) = (NetAddress)->NumBits;                      \
        (Addr) = (* (ULONG *) ((NetAddress)->AddrBits));    \

```





## -see-also




<a href="https://msdn.microsoft.com/2dd2c01b-41f1-48e3-942b-954f7b2efac5">RTM_IPV4_GET_ADDR_AND_MASK</a>



<a href="https://msdn.microsoft.com/fdbc2030-3917-4920-848e-76b5d1dfcfef">RTM_IPV4_LEN_FROM_MASK</a>



<a href="https://msdn.microsoft.com/9a5d9ee0-8199-420b-9489-068d1171e647">RTM_IPV4_MAKE_NET_ADDRESS</a>



<a href="https://msdn.microsoft.com/7f4a67d9-e707-413e-8cc3-600eb7968b82">RTM_IPV4_MASK_FROM_LEN</a>



<a href="https://msdn.microsoft.com/c6f60346-51ff-4e1e-9edb-b326184f79cf">RTM_IPV4_SET_ADDR_AND_LEN</a>



<a href="https://msdn.microsoft.com/23849eed-309a-41b8-b853-1267806166fa">RTM_IPV4_SET_ADDR_AND_MASK</a>



<a href="https://msdn.microsoft.com/92c4e797-9b73-438d-b4df-9739fae9d5c8">RTM_NET_ADDRESS</a>
 

 

