---
UID: NF:textstor.ITextStoreAnchor.InsertEmbedded
title: ITextStoreAnchor::InsertEmbedded (textstor.h)
author: windows-sdk-content
description: ITextStoreAnchor::InsertEmbedded method
old-location: tsf\itextstoreanchor_insertembedded.htm
tech.root: TSF
ms.assetid: 414842cc-7c3e-4f5c-93ac-3bd0eda5293e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextStoreAnchor interface [Text Services Framework],InsertEmbedded method, ITextStoreAnchor.InsertEmbedded, ITextStoreAnchor::InsertEmbedded, InsertEmbedded, InsertEmbedded method [Text Services Framework], InsertEmbedded method [Text Services Framework],ITextStoreAnchor interface, textstor/ITextStoreAnchor::InsertEmbedded, tsf.itextstoreanchor_insertembedded
ms.topic: method
req.header: textstor.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Textstor.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Msctf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - msctf.dll
api_name:
 - ITextStoreAnchor.InsertEmbedded
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITextStoreAnchor::InsertEmbedded


## -description




## -parameters




### -param dwFlags [in]

Must be TS_IE_CORRECTION.


### -param paStart [in]

Pointer to the anchor at the start of the object to be inserted.


### -param paEnd [in]

Pointer to the anchor at the end of the object to be inserted.


### -param pDataObject [in]

Pointer to an <b>IDataObject</b> data object.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The method was unable to obtain a valid interface pointer to the start and/or end anchors.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One or more input parameters are invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
The application does not support embedded objects.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TS_E_FORMAT</b></dt>
</dl>
</td>
<td width="60%">
The application does not support the data type contained in <i>pDataObject</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TS_E_INVALIDPOS</b></dt>
</dl>
</td>
<td width="60%">
<i>paStart</i> and/or <i>paEnd</i> are not within the document.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TS_E_NOLOCK</b></dt>
</dl>
</td>
<td width="60%">
The caller does not have a read/write lock.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms688421(v=VS.85).aspx">IDataObject</a>



<a href="https://msdn.microsoft.com/62730a6d-4dc8-4207-9818-ab95e6537854">ITextStoreAnchor</a>



<a href="https://msdn.microsoft.com/722506fa-db83-49d3-9434-a4ad7b797ce2">ITextStoreAnchor::QueryInsertEmbedded
      </a>



<a href="https://msdn.microsoft.com/03beac03-cd09-4e03-b700-d96741e4932b">ITextStoreAnchor::SetText
      </a>



<a href="https://msdn.microsoft.com/b40ca931-d45c-4101-9380-bb2b3ad25fba">TS_CHAR_EMBEDDED
      </a>



<a href="https://msdn.microsoft.com/a455d712-42d5-472e-862d-85ae3ba9149f">TS_IE_* Constants
      </a>
 

 

