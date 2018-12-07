---
UID: NF:bits3_0.IBitsPeerCacheAdministration.EnumRecords
title: IBitsPeerCacheAdministration::EnumRecords
author: windows-sdk-content
description: Gets an IEnumBitsPeerCacheRecords interface pointer that you use to enumerate the records in the cache. The enumeration is a snapshot of the records in the cache.
old-location: bits\ibitspeercacheadministration_enumrecords.htm
tech.root: bits
ms.assetid: b471cee0-0ad0-4488-9819-e524e50dbc76
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnumRecords, EnumRecords method [BITS], EnumRecords method [BITS],IBitsPeerCacheAdministration interface, IBitsPeerCacheAdministration interface [BITS],EnumRecords method, IBitsPeerCacheAdministration.EnumRecords, IBitsPeerCacheAdministration::EnumRecords, bits.ibitspeercacheadministration_enumrecords, bits3_0/IBitsPeerCacheAdministration::EnumRecords
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: bits3_0.h
req.include-header: Bits.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits3_0.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Bits.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Bits.lib
 - Bits.dll
api_name:
 - IBitsPeerCacheAdministration.EnumRecords
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBitsPeerCacheAdministration::EnumRecords


## -description


Gets an <a href="https://msdn.microsoft.com/en-us/library/Aa964302(v=VS.85).aspx">IEnumBitsPeerCacheRecords</a> interface pointer that you use to enumerate the records in the cache. The enumeration is a snapshot of the records in the cache.


## -parameters




### -param ppEnum [out]

An <a href="https://msdn.microsoft.com/en-us/library/Aa964302(v=VS.85).aspx">IEnumBitsPeerCacheRecords</a> interface pointer that you use to enumerate the records in the cache. Release <i>ppEnum</i> when done.


## -returns



This method returns S_OK on success or one of the standard COM <b>HRESULT</b> values on error.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa964272(v=VS.85).aspx">IBitsPeerCacheAdministration</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa964273(v=VS.85).aspx">IBitsPeerCacheAdministration::ClearPeers</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa964287(v=VS.85).aspx">IBitsPeerCacheAdministration::GetRecord</a>
 

 

