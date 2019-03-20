---
UID: NF:tom.ITextRow.SetAlignment
title: ITextRow::SetAlignment (tom.h)
author: windows-sdk-content
description: Sets the horizontal alignment of a row.
old-location: controls\itextrow_setalignment.htm
tech.root: Controls
ms.assetid: bfcc900d-2bec-4314-a2c5-09f55e27a626
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextRow interface [Windows Controls],SetAlignment method, ITextRow.SetAlignment, ITextRow::SetAlignment, SetAlignment, SetAlignment method [Windows Controls], SetAlignment method [Windows Controls],ITextRow interface, controls.itextrow_setalignment, tom/ITextRow::SetAlignment
ms.topic: method
req.header: tom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextRow.SetAlignment
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextRow::SetAlignment


## -description


Sets the horizontal alignment of a row.


## -parameters




### -param Value [in]

Type: <b>long</b>

The new horizontal alignment. It can be one of the following values.

<p class="indent"><a href="https://msdn.microsoft.com/en-us/library/Hh768766(v=VS.85).aspx">tomAlignLeft</a>

<p class="indent"><a href="https://msdn.microsoft.com/en-us/library/Hh768766(v=VS.85).aspx">tomAlignCenter</a>

<p class="indent"><a href="https://msdn.microsoft.com/en-us/library/Hh768766(v=VS.85).aspx">tomAlignRight</a>


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the method succeeds, it returns <b>NOERROR</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/49f5ffc1-d615-4d07-9f41-1c5f0dd9045b">ITextRow</a>



<a href="https://msdn.microsoft.com/2c7279b0-6329-4abd-a719-da4ed4d71c71">ITextRow::GetAlignment</a>
 

 

