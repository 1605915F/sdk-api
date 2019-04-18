---
UID: NS:clusapi.CLUSPROP_WORD
title: CLUSPROP_WORD (clusapi.h)
author: windows-sdk-content
description: Describes numeric data.
old-location: mscs\clusprop_word.htm
tech.root: MsCS
ms.assetid: ba09290b-171b-45cf-a367-485f7322ebef
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PCLUSPROP_WORD, CLUSPROP_WORD, CLUSPROP_WORD structure [Failover Cluster], PCLUSPROP_WORD, PCLUSPROP_WORD structure pointer [Failover Cluster], _wolf_clusprop_word, clusapi/CLUSPROP_WORD, clusapi/PCLUSPROP_WORD, mscs.clusprop_word"
ms.topic: struct
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Datacenter, Windows Server 2008 Enterprise
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
 - ClusAPI.h
api_name:
 - CLUSPROP_WORD
product: Windows
targetos: Windows
req.typenames: CLUSPROP_WORD, *PCLUSPROP_WORD
req.redist: 
ms.custom: 19H1
---

# CLUSPROP_WORD structure


## -description


Describes numeric data. It 
    is used as an entry in a <a href="https://msdn.microsoft.com/f2b20fe5-0d7e-4ccd-b288-aa8104a24fef">value list</a> and consists of:
<ul>
<li>A <a href="https://msdn.microsoft.com/a77a51aa-2d2a-4b21-9f87-87dcf95fa0cd">CLUSPROP_VALUE</a> structure describing the format, 
     type, and length of the numeric data.</li>
<li>A <b>WORD</b> value.</li>
</ul>

## -struct-fields




### -field w

Numeric value.


### -field CLUSPROP_VALUE


<a href="https://msdn.microsoft.com/a77a51aa-2d2a-4b21-9f87-87dcf95fa0cd">CLUSPROP_VALUE</a> structure describing 
       the format, type, and 
       the count of bytes in the <b>w</b> member. 


## -see-also




<a href="https://msdn.microsoft.com/23353e11-63bb-4d3b-90fb-e2a5544e0d09">CLUSPROP_SYNTAX</a>



<a href="https://msdn.microsoft.com/a77a51aa-2d2a-4b21-9f87-87dcf95fa0cd">CLUSPROP_VALUE</a>



<a href="https://msdn.microsoft.com/e3ad7c34-0c8a-4f03-8e5c-b57802c493f0">Data structures</a>
 

 

