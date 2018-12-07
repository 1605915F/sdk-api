---
UID: NF:certexit.ICertExit.GetDescription
title: ICertExit::GetDescription
author: windows-sdk-content
description: Returns a human-readable description of the exit module and its function.
old-location: security\icertexit2_getdescription.htm
tech.root: seccrypto
ms.assetid: 362d67c7-54ab-482e-9b2b-05ba1b6e2a70
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CCertExit object [Security],GetDescription method, GetDescription, GetDescription method [Security], GetDescription method [Security],CCertExit object, GetDescription method [Security],ICertExit interface, GetDescription method [Security],ICertExit2 interface, ICertExit interface [Security],GetDescription method, ICertExit.GetDescription, ICertExit2 interface [Security],GetDescription method, ICertExit2::GetDescription, ICertExit::GetDescription, _certsrv_icertexit_getdescription, certexit/ICertExit2::GetDescription, certexit/ICertExit::GetDescription, security.icertexit2_getdescription
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certexit.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certexit.h
api_name:
 - ICertExit2.GetDescription
 - ICertExit.GetDescription
 - CCertExit.GetDescription
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertExit::GetDescription


## -description


The <b>GetDescription</b> method returns a human-readable description of the exit module and its function. This method was first defined in the  <a href="https://msdn.microsoft.com/en-us/library/Aa385021(v=VS.85).aspx">ICertExit</a> interface.


## -parameters




### -param pstrDescription [out]

A pointer to the <b>BSTR</b> that describes the exit module.


## -returns



<h3>C++</h3>
 If the method succeeds, the method returns S_OK.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<h3>VB</h3>
 Returns a string that describes the exit module and its function.




## -remarks



When you write a custom exit module, implement this method.


#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>STDMETHODIMP
CCertExit::GetDescription(
    /* [out, retval] */ BSTR __RPC_FAR *pstrDescription)
{
    if (NULL == pstrDescription)
    {
        // Bad pointer address.
        return (E_POINTER);
    }
    if (NULL != *pstrDescription)
    {
        SysFreeString(*pstrDescription);
        *pstrDescription=NULL;
    }
    // wszMyExitModuleDesc defined elsewhere, for example:
    // #define wszMyExitModuleDesc L"My Exit Module"
    *pstrDescription = SysAllocString(wszMyExitModuleDesc);
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




<a href="https://msdn.microsoft.com/en-us/library/Aa385021(v=VS.85).aspx">ICertExit</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa385022(v=VS.85).aspx">ICertExit2</a>
 

 

