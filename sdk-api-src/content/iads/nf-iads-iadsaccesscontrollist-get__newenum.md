---
UID: NF:iads.IADsAccessControlList.get__NewEnum
title: IADsAccessControlList::get__NewEnum
author: windows-sdk-content
description: The IADsAccessControlList::get__NewEnum method is used to obtain an enumerator object for the ACL to enumerate ACEs.
old-location: adsi\iadsaccesscontrollist_get__newenum.htm
tech.root: adsi
ms.assetid: 569f3bfa-3933-43b3-9d16-c3d4382cfa9f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IADsAccessControlList interface [ADSI],get__NewEnum method, IADsAccessControlList.get__NewEnum, IADsAccessControlList::get__NewEnum, _ds_iadsaccesscontrollist_get__newenum, adsi.iadsaccesscontrollist__get____newenum, adsi.iadsaccesscontrollist_get__newenum, get__NewEnum, get__NewEnum method [ADSI], get__NewEnum method [ADSI],IADsAccessControlList interface, iads/IADsAccessControlList::get__NewEnum
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: iads.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: Activeds.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Activeds.dll
api_name:
 - IADsAccessControlList.get__NewEnum
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IADsAccessControlList::get__NewEnum


## -description


The <b>IADsAccessControlList::get__NewEnum</b> method is used to obtain an enumerator object for the ACL to enumerate ACEs.


## -parameters




### -param retval [out]

Pointer to pointer to the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface used to retrieve
      <a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a> interface on an enumerator object for the ACL.


## -returns



This method returns the standard return values, including <b>S_OK</b> and <b>E_FAIL</b>. For more information about other return values, see  <a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>.




## -remarks



Be aware  that there are two underscores in <b>get__NewEnum</b>.


#### Examples

The following code example makes an implicit call to the <b>get__NewEnum</b> method in the execution of the <b>For Each</b> loop.

<div class="code"><span codelanguage="VisualBasic"><table>
<tr>
<th>VB</th>
</tr>
<tr>
<td>
<pre>Dim Dacl As IADsAccessControlList
Dim ace As IADsAccessControlEntry

On Error GoTo Cleanup

' Get DACL. Code omitted.

' Display the trustees for each of the ACEs
For Each ace In Dacl 
    Debug.Print ace.trustee
Next ace

Cleanup:
    If (Err.Number&lt;&gt;0) Then
        MsgBox("An error has occurred. " &amp; Err.Number)
    End If
    Set Dacl = Nothing
    Set ace = Nothing
</pre>
</td>
</tr>
</table></span></div>
The following code example shows how to enumerate ACEs using <b>IADsAccessControlList::get__NewEnum</b>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>HRESULT ListTrustees(IADsAccessControlList *pACL)
{
    IEnumVARIANT *pEnum = NULL;
    LPUNKNOWN     pUnk = NULL;
    ULONG  lFetch = 0;
    BSTR    bstr = NULL;
    IADsAccessControlEntry *pACE = NULL;
    IDispatch *pDisp = NULL;
    VARIANT var;
    HRESULT hr = S_OK;
    
    VariantInit(&amp;var);
     
    hr = pACL-&gt;get__NewEnum(&amp;pUnk);
    if (FAILED(hr)){goto Cleanup;}
    
    hr = pUnk-&gt;QueryInterface( IID_IEnumVARIANT, (void**) &amp;pEnum );
    pUnk-&gt;Release();
    if (FAILED(hr)){goto Cleanup;}
     
    hr = pEnum-&gt;Next( 1, &amp;var, &amp;lFetch );
    if (FAILED(hr)){goto Cleanup;}
     
    while( hr == S_OK )
    {
        if ( lFetch == 1 )
        {
            if ( VT_DISPATCH != V_VT(&amp;var) )
            {
                goto Cleanup;
            }
            pDisp = V_DISPATCH(&amp;var);
            /////////////////////////
            // Get the individual ACE
            /////////////////////////
            hr = pDisp-&gt;QueryInterface( IID_IADsAccessControlEntry,(void**)&amp;pACE ); 
            if ( SUCCEEDED(hr) )
            {
                pACE-&gt;get_Trustee(&amp;bstr);
                printf("\n %S:\n", bstr);
                //ACE manipulation here
                SysFreeString(bstr);
                pACE-&gt;Release();
            }
            pACE-&gt;Release();
            pDisp-&gt;Release();
            VariantClear(&amp;var);
        }
        hr = pEnum-&gt;Next( 1, &amp;var, &amp;lFetch );
    }
    Cleanup:        
        if(pEnum) pEnum-&gt;Release();
        if(pUnk) pUnk-&gt;Release();
        if(bstr) SysFreeString(bstr);
        if(pACE) pACE-&gt;Release();
        VariantClear(&amp;var);
        return hr;
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/6d2cd45b-0dc6-4bb3-9c41-014bec71f258">IADsAccessControlEntry</a>



<a href="https://msdn.microsoft.com/de92d9cc-bc9d-4dc5-aa79-01f4d3050c35">IADsAccessControlList</a>



<a href="https://msdn.microsoft.com/c77547ab-e666-4d72-b8ef-4b2f3d61ad38">IADsSecurityDescriptor</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a>
 

 

