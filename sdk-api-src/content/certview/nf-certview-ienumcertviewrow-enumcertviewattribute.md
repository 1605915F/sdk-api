---
UID: NF:certview.IEnumCERTVIEWROW.EnumCertViewAttribute
title: IEnumCERTVIEWROW::EnumCertViewAttribute
author: windows-sdk-content
description: Obtains an instance of an attribute-enumeration sequence for the current row of the row-enumeration sequence.
old-location: security\ienumcertviewrow_enumcertviewattribute.htm
tech.root: seccrypto
ms.assetid: 53a70f66-3805-429e-8ef6-01b00b666b72
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnumCertViewAttribute, EnumCertViewAttribute method [Security], EnumCertViewAttribute method [Security],IEnumCERTVIEWROW interface, IEnumCERTVIEWROW interface [Security],EnumCertViewAttribute method, IEnumCERTVIEWROW.EnumCertViewAttribute, IEnumCERTVIEWROW::EnumCertViewAttribute, _certsrv_ienumcertviewrow_enumcertviewattribute, certview/IEnumCERTVIEWROW::EnumCertViewAttribute, security.ienumcertviewrow_enumcertviewattribute
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
 - IEnumCERTVIEWROW.EnumCertViewAttribute
 - IEnumCERTVIEWROW.EnumCertViewAttribute
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumCERTVIEWROW::EnumCertViewAttribute


## -description


The <b>EnumCertViewAttribute</b> method obtains an instance of an attribute-enumeration sequence for the current row of the row-enumeration sequence.


## -parameters




### -param Flags [in]

<table>
<tr>
<td><strong>C++</strong></td>
<td>
A <b>LONG</b> value. Must be zero.

</td>
</tr>
<tr>
<td><strong>VB</strong></td>
<td>
A <b>Long</b> value. Must be zero.

</td>
</tr>
</table>

### -param ppenum [out]

A pointer to a pointer of <a href="https://msdn.microsoft.com/en-us/library/Aa386157(v=VS.85).aspx">IEnumCERTVIEWATTRIBUTE</a> type. Upon successful completion of this method, <i>ppenum</i> is set to a pointer of <b>IEnumCERTVIEWATTRIBUTE</b> type.


## -returns



<h3>C++</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<h3>VB</h3>
 The returned value is an attribute-enumeration sequence object.




## -remarks



The 
attribute-enumeration sequence obtained by this call can be used to enumerate the attributes associated with the certificate in the current row. This enumeration can be accessed through the methods of the <a href="https://msdn.microsoft.com/en-us/library/Aa386157(v=VS.85).aspx">IEnumCERTVIEWATTRIBUTE</a> interface.

To reference a different row, call one of the following methods to navigate through the row-enumeration sequence:

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386255(v=VS.85).aspx">IEnumCERTVIEWROW::Reset</a>: Moves to the beginning of the enumeration sequence.</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386249(v=VS.85).aspx">IEnumCERTVIEWROW::Next</a>: Moves to the next row in the enumeration sequence.</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386260(v=VS.85).aspx">IEnumCERTVIEWROW::Skip</a>: Skips a specified number of rows.</li>
</ul>

#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>// pEnumRow is previously instantiated pointer to IEnumCERTVIEWROW
HRESULT                  hr;
LONG                     Index;
IEnumCERTVIEWATTRIBUTE * pEnumAttr = NULL;

// obtain enumerator for attributes
hr = pEnumRow-&gt;EnumCertViewAttribute(0, &amp;pEnumAttr);
if (FAILED(hr))
{
    printf("Failed EnumCertViewAttribute - %x\n", hr);
    goto error;
}
// enumerate each attribute
while (S_OK == pEnumAttr-&gt;Next(&amp;Index))
{
    // Use this attribute as needed.
}
error:

// Free resources.
if (NULL != pEnumAttr)
    pEnumAttr-&gt;Release();</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa386157(v=VS.85).aspx">IEnumCERTVIEWATTRIBUTE</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386231(v=VS.85).aspx">IEnumCERTVIEWROW</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386249(v=VS.85).aspx">IEnumCERTVIEWROW::Next</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386255(v=VS.85).aspx">IEnumCERTVIEWROW::Reset</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386260(v=VS.85).aspx">IEnumCERTVIEWROW::Skip</a>
 

 

