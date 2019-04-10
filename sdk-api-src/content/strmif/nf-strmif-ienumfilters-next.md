---
UID: NF:strmif.IEnumFilters.Next
title: IEnumFilters::Next (strmif.h)
author: windows-sdk-content
description: The Next method retrieves the specified number of filters in the enumeration sequence.
old-location: dshow\ienumfilters_next.htm
tech.root: DirectShow
ms.assetid: 0e376a01-d353-434c-864a-8001c8022679
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IEnumFilters interface [DirectShow],Next method, IEnumFilters.Next, IEnumFilters::Next, IEnumFiltersNext, Next, Next method [DirectShow], Next method [DirectShow],IEnumFilters interface, dshow.ienumfilters_next, strmif/IEnumFilters::Next
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - IEnumFilters.Next
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumFilters::Next


## -description



The <code>Next</code> method retrieves the specified number of filters in the enumeration sequence.




## -parameters




### -param cFilters [in]

Number of filters to retrieve.


### -param ppFilter [out]

Array of size <i>cFilters</i> that is filled with <a href="https://msdn.microsoft.com/d8c09dc7-dae8-4b51-8da8-69e64928a091">IBaseFilter</a> interface pointers. The caller must release the interfaces.


### -param pcFetched [out]

Receives the number of filters retrieved. Can be <b>NULL</b> if <i>cFilters</i> is 1.


## -returns



<table>
<tr>
<th>Value
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>S_FALSE</td>
<td>Did not retrieve as many filters as requested.</td>
</tr>
<tr>
<td>S_OK</td>
<td>Success.</td>
</tr>
<tr>
<td>E_INVALIDARG</td>
<td>Invalid argument.</td>
</tr>
<tr>
<td>E_POINTER</td>
<td><b>NULL</b> pointer argument.</td>
</tr>
<tr>
<td>VFW_E_ENUM_OUT_OF_SYNC</td>
<td>The graph has changed and is now inconsistent with the enumerator.</td>
</tr>
</table>
 




## -remarks



If the method succeeds, the <b>IBaseFilter</b> pointers all have outstanding reference counts. Be sure to release them when you are done.

If the filter graph changes (for example, the application removes a filter), the enumerator is no longer be consistent with the graph, and the method returns VFW_E_ENUM_OUT_OF_SYNC. Discard any data obtained from previous calls to the enumerator, because it might be invalid. Update the enumerator by calling the <a href="https://msdn.microsoft.com/997a6e56-cd11-42bf-b12c-a4418a4dc644">IEnumFilters::Reset</a> method. You can then call the <code>Next</code> method safely.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/e105ccff-86c6-45d5-aead-6d303d038e5a">IEnumFilters Interface</a>
 

 

