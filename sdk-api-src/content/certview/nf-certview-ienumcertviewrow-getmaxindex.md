---
UID: NF:certview.IEnumCERTVIEWROW.GetMaxIndex
title: IEnumCERTVIEWROW::GetMaxIndex
author: windows-sdk-content
description: Retrieves the maximum valid index value after all the rows in the row-enumeration sequence have been referenced.
old-location: security\ienumcertviewrow_getmaxindex.htm
tech.root: seccrypto
ms.assetid: 65ba80db-b7ee-46fa-b044-eab554720ce9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetMaxIndex, GetMaxIndex method [Security], GetMaxIndex method [Security],IEnumCERTVIEWROW interface, IEnumCERTVIEWROW interface [Security],GetMaxIndex method, IEnumCERTVIEWROW.GetMaxIndex, IEnumCERTVIEWROW::GetMaxIndex, certview/IEnumCERTVIEWROW::GetMaxIndex, security.ienumcertviewrow_getmaxindex, security.ienumcertviewrow_getmaxtindex
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certview.h
req.include-header: Certsrv.h
req.target-type: Windows
req.target-min-winverclnt: None supported
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
req.lib: Certidl.lib
req.dll: Certadm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certadm.dll
api_name:
 - IEnumCERTVIEWROW.GetMaxIndex
 - IEnumCERTVIEWROW.GetMaxIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumCERTVIEWROW::GetMaxIndex


## -description


The <b>GetMaxIndex</b> method retrieves the maximum valid index value after all the rows in the row-enumeration sequence have been referenced.


## -parameters




### -param pIndex [out]

A pointer to a <b>LONG</b> variable that contains the maximum index value for the row-enumeration sequence. This method fails if <i>pIndex</i> is <b>NULL</b>.


## -returns



<h3>C++</h3>
 If the method succeeds, the method returns S_OK and <i>pIndex</i> is set to the maximum index value for the row-enumeration sequence.

If traversal to the last row has not occurred, this method fails with a return value of E_UNEXPECTED.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<h3>VB</h3>
 The return value is the maximum index value for the row-enumeration sequence. This method fails if traversal to the last row has not occurred.




## -remarks



Successful completion of this method is dependent on reaching the last row of the enumeration sequence. The maximum row index can be useful to size a scroll bar or display window, but it can also be resource-intensive to compute because it requires evaluating the entire query. For some queries, column data for each row must be examined to determine whether it is included in the view. After the user has paged through all of the data or explicitly requested to proceed to the end, the maximum row index is preserved.

To navigate through the row-enumeration sequence, call the following methods.

<table>
<tr>
<th>Method</th>
<th>Description</th>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Aa386255(v=VS.85).aspx">IEnumCERTVIEWROW::Reset</a>
</td>
<td>Moves to the beginning of the enumeration sequence.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Aa386249(v=VS.85).aspx">IEnumCERTVIEWROW::Next</a>
</td>
<td>Moves to the next row in the enumeration sequence.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Aa386260(v=VS.85).aspx">IEnumCERTVIEWROW::Skip</a>
</td>
<td>Skips a specified number of rows.</td>
</tr>
</table>
 


#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#include &lt;windows.h&gt;
#include &lt;stdio.h&gt;
#include &lt;Certview.h&gt;

long nMax;

//  Determine the maximum row index.
hr = pRow-&gt;GetMaxIndex(&amp;nMax);
if (FAILED(hr))
    printf("Failed GetMaxIndex [%x]\n", hr);
else
    printf("Max index is: %d\n", nMax);
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>IEnumCERTVIEWROW</b>



<a href="https://msdn.microsoft.com/en-us/library/Aa386249(v=VS.85).aspx">IEnumCERTVIEWROW::Next</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386255(v=VS.85).aspx">IEnumCERTVIEWROW::Reset</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386260(v=VS.85).aspx">IEnumCERTVIEWROW::Skip</a>
 

 

