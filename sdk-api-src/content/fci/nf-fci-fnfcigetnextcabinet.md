---
UID: NF:fci.FNFCIGETNEXTCABINET
title: FNFCIGETNEXTCABINET macro
author: windows-sdk-content
description: The FNFCIGETNEXTCABINET macro provides the declaration for the application-defined callback function to request information for the next cabinet.
old-location: winprog\fnfcigetnextcabinet.htm
tech.root: devnotes
ms.assetid: d56fb63e-91bf-4991-a954-176211697a2e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FNFCIGETNEXTCABINET, FNFCIGETNEXTCABINET macro [Windows API], fci/FNFCIGETNEXTCABINET, winprog.fnfcigetnextcabinet
ms.topic: macro
req.header: fci.h
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
 - fci.h
api_name:
 - FNFCIGETNEXTCABINET
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FNFCIGETNEXTCABINET macro


## -description


The <b>FNFCIGETNEXTCABINET</b> macro provides the declaration for the application-defined callback function to request information for the next cabinet.


## -parameters




### -param fn

Pointer to a <a href="https://msdn.microsoft.com/en-us/library/Ff797925(v=VS.85).aspx">CCAB</a> structure to provide the parameters for the creation of a new cabinet.


#### - cbPrevCab

Size, in bytes, of the previous cabinet.


#### - pv

Pointer to an application-defined value.


## -remarks



The <a href="https://msdn.microsoft.com/en-us/library/Ff797925(v=VS.85).aspx">CCAB</a> structure referenced by this function is relevant to the most recently completed cabinet. However, with each successful operation the  <i>iCab</i> field contained within this structure will have incremented by 1. Additionally, the next cabinet will be created using the fields in this structure.  The szCab, in particular, should be modified as necessary. In particular, the <i>szCab</i> field, which specifies the cabinet name, should be changed for each cabinet.

When creating multiple cabinets, typically the <i>iCab</i> field is used to create the name.


#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>FNFCIGETNEXTCABINET(fnGetNextCabinet)
{
    HRESULT hr;

    UNREFERENCED_PARAMETER(pv);
    UNREFERENCED_PARAMETER(cbPrevCab);
    
    hr = StringCchPrintfA(pccab-&gt;szCab,
                          ARRAYSIZE(pccab-&gt;szCab),
                          "FCISample%02d.cab",
                          pccab-&gt;iCab);
        
    return ( SUCCEEDED(hr) );
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/bfcea06d-2f09-405c-955c-0f56149148f2">FCICreate</a>
 

 

