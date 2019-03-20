---
UID: NF:mfmediaengine.IMFTimedTextRegion.GetLineHeight
title: IMFTimedTextRegion::GetLineHeight (mfmediaengine.h)
author: windows-sdk-content
description: Gets the height of each line of text in the region.
old-location: mf\imftimedtextregion_getlineheight.htm
tech.root: medfound
ms.assetid: 41514FCA-5C2A-48E5-A9F8-72B5B9160CD6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLineHeight, GetLineHeight method [Media Foundation], GetLineHeight method [Media Foundation],IMFTimedTextRegion interface, IMFTimedTextRegion interface [Media Foundation],GetLineHeight method, IMFTimedTextRegion.GetLineHeight, IMFTimedTextRegion::GetLineHeight, mf.imftimedtextregion_getlineheight, mfmediaengine/IMFTimedTextRegion::GetLineHeight
ms.topic: method
req.header: mfmediaengine.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mfmediaengine.idl
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
 - COM
api_location:
 - mfmediaengine.h
api_name:
 - IMFTimedTextRegion.GetLineHeight
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFTimedTextRegion::GetLineHeight


## -description


Gets the height of each line of text in the region.


## -parameters




### -param pLineHeight [out]

Type: <b>double*</b>

A pointer to a variable that receives the height of each line of text in the region.


### -param unitType [out]

Type: <b><a href="https://msdn.microsoft.com/5F811CEC-9E60-4441-BD22-1C4F4D0B72F8">MF_TIMED_TEXT_UNIT_TYPE</a>*</b>

A pointer to a variable that receives a <a href="https://msdn.microsoft.com/5F811CEC-9E60-4441-BD22-1C4F4D0B72F8">MF_TIMED_TEXT_UNIT_TYPE</a>-typed value that specifies the units in which the timed-text region is measured.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/1A6E068F-2E01-4A72-8BCF-D645B1D21ECF">IMFTimedTextRegion</a>
 

 

