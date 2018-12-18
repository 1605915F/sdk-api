---
UID: NF:traceloggingprovider.TRACELOGGING_DECLARE_PROVIDER
title: TRACELOGGING_DECLARE_PROVIDER macro
author: windows-sdk-content
description: Forward declares a global TraceLogging provider handle.
old-location: tracelogging\TRACELOGGING_DECLARE_PROVIDER.htm
tech.root: tracelogging
ms.assetid: E9C0B622-77A5-498F-BB28-C6C181271276
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TRACELOGGING_DECLARE_PROVIDER, TRACELOGGING_DECLARE_PROVIDER macro, tracelogging.TRACELOGGING_DECLARE_PROVIDER, tracelogging.traceloggingdeclareprovider, traceloggingprovider/TRACELOGGING_DECLARE_PROVIDER
ms.topic: macro
req.header: traceloggingprovider.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2012 R2
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
 - traceloggingprovider.h
api_name:
 - TRACELOGGING_DECLARE_PROVIDER
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TRACELOGGING_DECLARE_PROVIDER macro


## -description


Forward declares a global TraceLogging provider handle.


## -parameters




### -param handleVariable [in]

The handle variable name to forward declare.


## -remarks



Use this macro in a shared header file to forward declare your TraceLogging provider handle. This macro does not allocate storage for the provider. In order to use the provider, you will need to use <a href="https://msdn.microsoft.com/4515652D-86B0-4274-8523-27292F5F6815">TRACELOGGING_DEFINE_PROVIDER</a> to define the variable.

If the header file that you use this macro in is used in both C and C++ code, you will need to
enclose TRACELOGGING_DECLARE_PROVIDER in an extern "C" region so
that the provider handle variable is declared as C-compatible. For example:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>    #ifdef __cplusplus
    extern "C" {
    #endif
    TRACELOGGING_DECLARE_PROVIDER(g_hMyProvider);
    #ifdef __cplusplus
    } // extern "C"
    #endif</pre>
</td>
</tr>
</table></span></div>


