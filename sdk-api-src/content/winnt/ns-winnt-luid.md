---
UID: NS:winnt._LUID
title: LUID (winnt.h)
author: windows-sdk-content
description: Describes a local identifier for an adapter.
old-location: direct3ddxgi\_luid.htm
tech.root: direct3ddxgi
ms.assetid: 00601551-D6CE-4164-BDAF-DBCCF197990E
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PLUID, LUID, LUID structure [DXGI], _LUID, direct3ddxgi._luid, winnt/LUID"
ms.topic: struct
req.header: winnt.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - winnt.h
api_name:
 - LUID
product: Windows
targetos: Windows
req.typenames: LUID, *PLUID
req.redist: 
---

# LUID structure


## -description


Describes a local identifier for an adapter.


## -struct-fields




### -field LowPart

Specifies a DWORD that contains the unsigned lower numbers of the id.


### -field HighPart

Specifies a LONG that contains the signed high numbers of the id.


## -remarks



This structure is used by the <a href="https://msdn.microsoft.com/006E72E0-AE09-4834-9ACB-D48698050BF2">ID3D12Device::GetAdapterLuid</a> and <a href="https://msdn.microsoft.com/278F1C2B-6DE7-4D4A-8C6E-10B1004B8EFC">GetSharedResourceAdapterLuid</a> methods.
        




## -see-also




<a href="https://msdn.microsoft.com/22e98880-bcd1-448a-9223-604fff9173fe">DXGI Structures</a>
 

 

