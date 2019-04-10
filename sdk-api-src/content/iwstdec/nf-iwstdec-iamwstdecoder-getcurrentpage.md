---
UID: NF:iwstdec.IAMWstDecoder.GetCurrentPage
title: IAMWstDecoder::GetCurrentPage (iwstdec.h)
author: windows-sdk-content
description: Downstream filters use the GetCurrentPage method to retrieve the current WST page.
old-location: dshow\iamwstdecoder_getcurrentpage.htm
tech.root: DirectShow
ms.assetid: e4e52723-27ad-487a-a547-7ad7ade6f099
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetCurrentPage, GetCurrentPage method [DirectShow], GetCurrentPage method [DirectShow],IAMWstDecoder interface, IAMWstDecoder interface [DirectShow],GetCurrentPage method, IAMWstDecoder.GetCurrentPage, IAMWstDecoder::GetCurrentPage, IAMWstDecoderGetCurrentPage, dshow.iamwstdecoder_getcurrentpage, iwstdec/IAMWstDecoder::GetCurrentPage
ms.topic: method
req.header: iwstdec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IAMWstDecoder.GetCurrentPage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMWstDecoder::GetCurrentPage


## -description



Downstream filters use the <code>GetCurrentPage</code> method to retrieve the current WST page.




## -parameters




### -param pWstPage [out]

A pointer to an <a href="https://msdn.microsoft.com/en-us/library/Dd373508(v=VS.85).aspx">AM_WST_PAGE</a> structure to receive the current page.


## -returns



When the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376041(v=VS.85).aspx">IAMWstDecoder Interface</a>
 

 

