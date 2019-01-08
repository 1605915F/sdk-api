---
UID: NF:certpol.ICertPolicy.GetDescription
title: ICertPolicy::GetDescription
author: windows-sdk-content
description: Returns a human-readable description of the policy module and its function.
old-location: security\icertpolicy2_getdescription.htm
tech.root: SecCrypto
ms.assetid: 38b85fa8-f5e7-4ac8-9f38-1cad83417797
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CCertPolicy object [Security],GetDescription method, GetDescription, GetDescription method [Security], GetDescription method [Security],CCertPolicy object, GetDescription method [Security],ICertPolicy interface, GetDescription method [Security],ICertPolicy2 interface, ICertPolicy interface [Security],GetDescription method, ICertPolicy.GetDescription, ICertPolicy2 interface [Security],GetDescription method, ICertPolicy2::GetDescription, ICertPolicy::GetDescription, _certsrv_icertpolicy_getdescription, certpol/ICertPolicy2::GetDescription, certpol/ICertPolicy::GetDescription, security.icertpolicy2_getdescription
ms.topic: method
req.header: certpol.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certidl.lib
 - Certidl.dll
api_name:
 - ICertPolicy2.GetDescription
 - ICertPolicy.GetDescription
 - CCertPolicy.GetDescription
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertPolicy::GetDescription


## -description


The <b>GetDescription</b> method returns a human-readable description of the policy module and its function.


## -parameters




### -param pstrDescription [out]

A pointer to a <b>BSTR</b> that describes the policy module.


## -returns



<h3>C++</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.

<h3>VB</h3>
 Returns a string that describes the policy module and its function.




## -remarks



When you write custom policy modules, implement this method.


#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#include &lt;windows.h&gt;
#include &lt;Certpol.h&gt;

STDMETHODIMP CCertPolicy::GetDescription(
    /* [out, retval] */ BSTR __RPC_FAR *pstrDescription)
{
    if (NULL == pstrDescription)
    {
        // Bad pointer address
        return ( E_POINTER );
    }
    if (NULL != *pstrDescription)
    {
        SysFreeString(*pstrDescription);
        *pstrDescription=NULL;
    }
    // wszMyModuleDesc defined elsewhere, for example:
    // #define wszMyModuleDesc L"My Policy Module"
    *pstrDescription = SysAllocString(wszMyModuleDesc);
    if (NULL == *pstrDescription)
    {
        // Not enough memory
        return ( E_OUTOFMEMORY );
    }
    // Success
    return( S_OK );
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/14031490-be8e-47f9-8c66-ae27f7d3599c">ICertPolicy</a>



<a href="https://msdn.microsoft.com/2e48b096-e23a-4106-bfaf-f089d2291fba">ICertPolicy2</a>
 

 

