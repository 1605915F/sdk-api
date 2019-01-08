---
UID: NF:certview.IEnumCERTVIEWCOLUMN.Reset
title: IEnumCERTVIEWCOLUMN::Reset
author: windows-sdk-content
description: Moves to the beginning of the column-enumeration sequence.
old-location: security\ienumcertviewcolumn_reset.htm
tech.root: SecCrypto
ms.assetid: 0be00eb0-1a22-4849-95ca-276099bbfa74
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumCERTVIEWCOLUMN interface [Security],Reset method, IEnumCERTVIEWCOLUMN object [Security],Reset method, IEnumCERTVIEWCOLUMN.Reset, IEnumCERTVIEWCOLUMN::Reset, Reset, Reset method [Security], Reset method [Security],IEnumCERTVIEWCOLUMN interface, Reset method [Security],IEnumCERTVIEWCOLUMN object, _certsrv_ienumcertviewcolumn_reset, certview/IEnumCERTVIEWCOLUMN::Reset, security.ienumcertviewcolumn_reset
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
 - IEnumCERTVIEWCOLUMN.Reset
 - IEnumCERTVIEWCOLUMN.Reset
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumCERTVIEWCOLUMN::Reset


## -description


The <b>Reset</b> method moves to the beginning of the column-enumeration sequence.


## -parameters






## -returns



<h3>VB</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.




## -remarks



Upon successful completion of this method, call the 
<a href="https://msdn.microsoft.com/4c77d1c7-af3a-4a7d-bf42-69be887c881e">IEnumCERTVIEWCOLUMN::Next</a> method to reference the first column in the enumeration. After this second call is made, the information in the column can be obtained by calling one of the following methods:

<ul>
<li>
<a href="https://msdn.microsoft.com/be76cec1-9ac0-4cc0-bddb-992b2d3590d7">IEnumCERTVIEWCOLUMN::GetName</a>: Retrieves the nonlocalized name of the column.</li>
<li>
<a href="https://msdn.microsoft.com/e7fd06f7-7b42-47ed-be03-867d0d03594a">IEnumCERTVIEWCOLUMN::GetDisplayName</a>: Retrieves the localized name of the column.</li>
<li>
<a href="https://msdn.microsoft.com/5cc14bd1-7963-4b11-aef6-4ef3b0b7f6c1">IEnumCERTVIEWCOLUMN::GetValue</a>: Retrieves the data in the column.</li>
<li>
<a href="https://msdn.microsoft.com/53297e9e-6583-4edf-85f4-e2b2e4ba28b3">IEnumCERTVIEWCOLUMN::GetType</a>: Retrieves the type of data in the column.</li>
<li>
<a href="https://msdn.microsoft.com/20cd5f5a-2e19-43ca-9b84-70e6dd1a4cad">IEnumCERTVIEWCOLUMN::GetMaxLength</a>: Retrieves the maximum length, in bytes, of the column.</li>
</ul>

#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>// pEnumCol is previously instantiated IEnumCERTVIEWCOLUMN object
HRESULT    hr;
LONG        Index;
hr = pEnumCol-&gt;Reset();
if (S_OK != hr)
    printf("Unable to reset pEnumCol\n");
    // call appropriate error handler / exit routine
else
{
    // now at the beginning of the columns
    // enumerate each column
    while (S_OK == pEnumCol-&gt;Next(&amp;Index))
    {
        // Use each column as needed.
    }
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/6e6547f9-44b2-4050-be90-ac8ede892adc">IEnumCERTVIEWCOLUMN</a>



<a href="https://msdn.microsoft.com/e7fd06f7-7b42-47ed-be03-867d0d03594a">IEnumCERTVIEWCOLUMN::GetDisplayName</a>



<a href="https://msdn.microsoft.com/20cd5f5a-2e19-43ca-9b84-70e6dd1a4cad">IEnumCERTVIEWCOLUMN::GetMaxLength</a>



<a href="https://msdn.microsoft.com/be76cec1-9ac0-4cc0-bddb-992b2d3590d7">IEnumCERTVIEWCOLUMN::GetName</a>



<a href="https://msdn.microsoft.com/53297e9e-6583-4edf-85f4-e2b2e4ba28b3">IEnumCERTVIEWCOLUMN::GetType</a>



<a href="https://msdn.microsoft.com/5cc14bd1-7963-4b11-aef6-4ef3b0b7f6c1">IEnumCERTVIEWCOLUMN::GetValue</a>
 

 

