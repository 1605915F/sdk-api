---
UID: NF:certview.IEnumCERTVIEWROW.Reset
title: IEnumCERTVIEWROW::Reset
author: windows-sdk-content
description: Moves to the beginning of the row-enumeration sequence.
old-location: security\ienumcertviewrow_reset.htm
tech.root: seccrypto
ms.assetid: 76bee5db-0443-4673-a59c-0198587736dc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumCERTVIEWROW interface [Security],Reset method, IEnumCERTVIEWROW object [Security],Reset method, IEnumCERTVIEWROW.Reset, IEnumCERTVIEWROW::Reset, Reset, Reset method [Security], Reset method [Security],IEnumCERTVIEWROW interface, Reset method [Security],IEnumCERTVIEWROW object, _certsrv_ienumcertviewrow_reset, certview/IEnumCERTVIEWROW::Reset, security.ienumcertviewrow_reset
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
 - IEnumCERTVIEWROW.Reset
 - IEnumCERTVIEWROW.Reset
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumCERTVIEWROW::Reset


## -description


The <b>Reset</b> method moves to the beginning of the row-enumeration sequence.


## -parameters






## -returns



<h3>VB</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.




## -remarks



Upon successful completion of this method, call the <a href="https://msdn.microsoft.com/en-us/library/Aa386249(v=VS.85).aspx">IEnumCERTVIEWROW::Next</a> method to reference the first row in the enumeration. 

After this second call is made, the 
columns, attributes, and extensions associated with the certificate in the row can be enumerated using the methods of the following interfaces:

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386176(v=VS.85).aspx">IEnumCERTVIEWCOLUMN</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386157(v=VS.85).aspx">IEnumCERTVIEWATTRIBUTE</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa386203(v=VS.85).aspx">IEnumCERTVIEWEXTENSION</a>
</li>
</ul>

#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>// pEnumRow is previously instantiated pointer to IEnumCERTVIEWROW.
HRESULT hr;
LONG    Index;

// Ensure enumerator is at first row.
hr = pEnumRow-&gt;Reset();
if (FAILED(hr))
    printf("Failed to Reset\n");
else
{
    printf("Reset to beginning\n");
    // Retrieve first record.
    hr = pEnumRow-&gt;Next(&amp;Index);
    // Examine hr for success and process row.
    // ...
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa386157(v=VS.85).aspx">IEnumCERTVIEWATTRIBUTE</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386176(v=VS.85).aspx">IEnumCERTVIEWCOLUMN</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386203(v=VS.85).aspx">IEnumCERTVIEWEXTENSION</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa386231(v=VS.85).aspx">IEnumCERTVIEWROW</a>
 

 

