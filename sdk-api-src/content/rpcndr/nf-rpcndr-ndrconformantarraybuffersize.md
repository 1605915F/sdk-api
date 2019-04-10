---
UID: NF:rpcndr.NdrConformantArrayBufferSize
title: NdrConformantArrayBufferSize function (rpcndr.h)
author: windows-sdk-content
description: The NdrConformantArrayBufferSize function calculates the required buffer size, in bytes, to marshal the conformant array.
old-location: winprog\ndrcomformantarraybuffersize.htm
tech.root: DevNotes
ms.assetid: 0f230b58-6f80-40c1-b70d-5ba7fbb5a130
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: NdrComformantArrayBufferSize, NdrConformantArrayBufferSize, NdrConformantArrayBufferSize function [Windows API], rpcndr/NdrConformantArrayBufferSize, winprog.ndrcomformantarraybuffersize
ms.topic: function
req.header: rpcndr.h
req.include-header: 
req.target-type: Windows
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
req.lib: Rpcrt4.lib
req.dll: Rpcrt4.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Rpcrt4.dll
api_name:
 - NdrConformantArrayBufferSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# NdrConformantArrayBufferSize function


## -description


The <b>NdrConformantArrayBufferSize</b> function calculates the required buffer size, in bytes, to marshal the conformant array.


## -parameters




### -param pStubMsg [in, out]

Pointer to a <a href="https://msdn.microsoft.com/9bd021f6-10c9-4e77-be75-9a89a3a016e0">MIDL_STUB_MESSAGE</a> structure that maintains the current status of the RPC stub. The <b>BufferLength</b> member contains the size of the buffer. The <b>MIDL_STUB_MESSAGE</b> structure is for internal use only, and must not be modified. 


### -param pMemory [in]

Pointer to the conformant array to be calculated.


### -param pFormat [in]

Pointer to the format string description.


## -returns



This function has no return values. 




## -see-also




<a href="https://msdn.microsoft.com/9bd021f6-10c9-4e77-be75-9a89a3a016e0">MIDL_STUB_MESSAGE</a>
 

 

