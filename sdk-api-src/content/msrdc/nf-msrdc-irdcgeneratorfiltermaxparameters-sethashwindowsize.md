---
UID: NF:msrdc.IRdcGeneratorFilterMaxParameters.SetHashWindowSize
title: IRdcGeneratorFilterMaxParameters::SetHashWindowSize
author: windows-sdk-content
description: Sets the hash window size&#8212;the size of the sliding window used by the FilterMax generator for computing the hash used in the local maxima calculations.
old-location: rdc\irdcgeneratorfiltermaxparameters_sethashwindowsize.htm
tech.root: rdc
ms.assetid: b18a5db1-f480-46c4-bac3-b0b2f0da6cfa
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IRdcGeneratorFilterMaxParameters interface [Remote Differential Compression],SetHashWindowSize method, IRdcGeneratorFilterMaxParameters.SetHashWindowSize, IRdcGeneratorFilterMaxParameters::SetHashWindowSize, SetHashWindowSize, SetHashWindowSize method [Remote Differential Compression], SetHashWindowSize method [Remote Differential Compression],IRdcGeneratorFilterMaxParameters interface, fs.irdcgeneratorfiltermaxparameters_sethashwindowsize, msrdc/IRdcGeneratorFilterMaxParameters::SetHashWindowSize, rdc.irdcgeneratorfiltermaxparameters_sethashwindowsize
ms.topic: method
req.header: msrdc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: MsRdc.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: MsRdc.dll
req.lib: 
req.dll: MsRdc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - MsRdc.dll
api_name:
 - IRdcGeneratorFilterMaxParameters.SetHashWindowSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRdcGeneratorFilterMaxParameters::SetHashWindowSize


## -description


The <b>SetHashWindowSize</b> 
    method sets the hash window size—the size of the sliding window used by the 
    FilterMax generator for computing the hash used in the local maxima calculations.


## -parameters




### -param hashWindowSize [in]

The length in bytes of the hash window size. The valid range is from 
      <b>MSRDC_MINIMUM_HASHWINDOWSIZE</b> to 
      <b>MSRDC_MAXIMUM_HASHWINDOWSIZE</b>.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/c1a0460c-ca48-48ca-bd5b-1213e8279366">GetHashWindowSize</a>



<a href="https://msdn.microsoft.com/6767ab24-2bb6-48bf-8f12-794d8b22e2b7">IRdcGeneratorFilterMaxParameters</a>
 

 

