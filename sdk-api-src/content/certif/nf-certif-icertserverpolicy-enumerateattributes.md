---
UID: NF:certif.ICertServerPolicy.EnumerateAttributes
title: ICertServerPolicy::EnumerateAttributes
author: windows-sdk-content
description: Retrieves the name of the current attribute and moves the internal enumeration pointer to the next attribute.
old-location: security\icertserverpolicy_enumerateattributes.htm
tech.root: seccrypto
ms.assetid: 5db05ed9-ab17-462b-9a76-34458489771a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CCertServerPolicy object [Security],EnumerateAttributes method, EnumerateAttributes, EnumerateAttributes method [Security], EnumerateAttributes method [Security],CCertServerPolicy object, EnumerateAttributes method [Security],ICertServerPolicy interface, ICertServerPolicy interface [Security],EnumerateAttributes method, ICertServerPolicy.EnumerateAttributes, ICertServerPolicy::EnumerateAttributes, _certsrv_icertserverpolicy_enumerateattributes, certif/ICertServerPolicy::EnumerateAttributes, security.icertserverpolicy_enumerateattributes
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certif.h
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
req.dll: Certcli.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certcli.dll
api_name:
 - ICertServerPolicy.EnumerateAttributes
 - CCertServerPolicy.EnumerateAttributes
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertServerPolicy::EnumerateAttributes


## -description


The <b>EnumerateAttributes</b> method retrieves the name of the current attribute and moves the internal enumeration pointer to the next  attribute.


## -parameters




### -param pstrAttributeName [out]

A pointer to the attribute name.


## -returns



<h3>C++</h3>
 If the method succeeds, the method returns S_OK, and the <i>pstrAttributeName</i> parameter is set to a <b>BSTR</b> that contains the name of the  attribute. A value of S_FALSE is returned if the last attribute was already enumerated.

To use this method, create a variable of <b>BSTR</b> type, set the variable equal to <b>NULL</b>, and then pass the address of this variable as <i>pstrAttributeName</i>.

When you have finished using the <b>BSTR</b>, free it by calling the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function.

If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<h3>VB</h3>
 Returns a string that contains the name of the attribute, or an empty string if the last attribute was already enumerated.




## -remarks



Before calling the <b>EnumerateAttributes</b>  method for the first time, call 
the <a href="https://msdn.microsoft.com/en-us/library/Aa385083(v=VS.85).aspx">EnumerateAttributesSetup</a> method to initialize the enumeration pointer to the first attribute.

 When done enumerating, call  
the <a href="https://msdn.microsoft.com/en-us/library/Aa385082(v=VS.85).aspx">EnumerateAttributesClose</a> method to free resources used by the enumeration calls.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa385080(v=VS.85).aspx">ICertServerPolicy</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa385082(v=VS.85).aspx">ICertServerPolicy::EnumerateAttributesClose</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa385083(v=VS.85).aspx">ICertServerPolicy::EnumerateAttributesSetup</a>
 

 

