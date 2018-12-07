---
UID: NF:certview.IEnumCERTVIEWCOLUMN.GetDisplayName
title: IEnumCERTVIEWCOLUMN::GetDisplayName
author: windows-sdk-content
description: Retrieves the localized name of the current column in the column-enumeration sequence.
old-location: security\ienumcertviewcolumn_getdisplayname.htm
tech.root: seccrypto
ms.assetid: e7fd06f7-7b42-47ed-be03-867d0d03594a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDisplayName, GetDisplayName method [Security], GetDisplayName method [Security],IEnumCERTVIEWCOLUMN interface, IEnumCERTVIEWCOLUMN interface [Security],GetDisplayName method, IEnumCERTVIEWCOLUMN.GetDisplayName, IEnumCERTVIEWCOLUMN::GetDisplayName, _certsrv_ienumcertviewcolumn_getdisplayname, certview/IEnumCERTVIEWCOLUMN::GetDisplayName, security.ienumcertviewcolumn_getdisplayname
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
 - IEnumCERTVIEWCOLUMN.GetDisplayName
 - IEnumCERTVIEWCOLUMN.GetDisplayName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumCERTVIEWCOLUMN::GetDisplayName


## -description


The <b>GetDisplayName</b> method retrieves the localized name of the current column in the column-enumeration sequence.


## -parameters




### -param pstrOut [out]

A pointer to a variable of <b>BSTR</b> type that contains the localized name of the column.


## -returns



<h3>C++</h3>
 If the method succeeds, the method returns S_OK and the <i>pstrOut</i> parameter contains the localized name of the column.

To use this method, create a variable of <b>BSTR</b> type, set the variable equal to <b>NULL</b>, and pass the address of this variable as <i>pstrOut</i>. When you have finished using the <b>BSTR</b>, free it by calling the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<h3>VB</h3>
 The return value is a <b>String</b> that contains the localized name of the column.




## -remarks



This method is used to retrieve the localized name of the column currently referenced by the 
column-enumeration sequence.

If the column-enumeration sequence is  not referencing a valid column, <b>GetDisplayName</b> will fail. Use one of the following methods to navigate through the enumeration:

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386199(v=VS.85).aspx">IEnumCERTVIEWCOLUMN::Reset</a>: Moves to the beginning of the enumeration sequence.</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386197(v=VS.85).aspx">IEnumCERTVIEWCOLUMN::Next</a>: Moves to the next column in the enumeration sequence.</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386201(v=VS.85).aspx">IEnumCERTVIEWCOLUMN::Skip</a>: Skips a specified number of columns.</li>
</ul>

#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>BSTR     bstrDisplay = NULL;
HRESULT  hr;

// pEnumCol is previously instantiated IEnumCERTVIEWCOLUMN object.
hr = pEnumCol-&gt;GetDisplayName(&amp;bstrDisplay);
if (S_OK == hr)
    printf("Column name is %ws\n", bstrDisplay);

// Done processing, clear resources.
if (NULL != bstrDisplay)
    SysFreeString(bstrDisplay);</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa386176(v=VS.85).aspx">IEnumCERTVIEWCOLUMN</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386197(v=VS.85).aspx">IEnumCERTVIEWCOLUMN::Next</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386199(v=VS.85).aspx">IEnumCERTVIEWCOLUMN::Reset</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386201(v=VS.85).aspx">IEnumCERTVIEWCOLUMN::Skip</a>
 

 

