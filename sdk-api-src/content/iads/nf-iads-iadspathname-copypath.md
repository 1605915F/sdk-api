---
UID: NF:iads.IADsPathname.CopyPath
title: IADsPathname::CopyPath
author: windows-sdk-content
description: Creates a copy of the Pathname object.
old-location: adsi\iadspathname_copypath.htm
tech.root: adsi
ms.assetid: 00c4a0b8-4961-4ceb-86fe-5cdc4e0a45c0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CopyPath, CopyPath method [ADSI], CopyPath method [ADSI],IADsPathname interface, IADsPathname interface [ADSI],CopyPath method, IADsPathname.CopyPath, IADsPathname::CopyPath, _ds_iadspathname_copypath, adsi.iadspathname__copypath, adsi.iadspathname_copypath, iads/IADsPathname::CopyPath
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
 - IADsPathname.CopyPath
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IADsPathname::CopyPath


## -description


The <b>IADsPathname::CopyPath</b> method 
   creates a copy of the Pathname object.


## -parameters




### -param ppAdsPath [out]

The <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface pointer on the 
      returned <a href="https://msdn.microsoft.com/9aa26d6c-aa86-4a23-a986-b8cb9057772a">IADsPathname</a> object.


## -returns



This method supports the standard return values, as well as the following:

For more information and other return values, see <a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error 
       Codes</a>.




## -remarks



This method is used to modify the object path and retain the original object path.


#### Examples

The following Visual Basic code example shows how to make a copy of a pathname.


```vb
Dim x, y As New Pathname
x.Set "LDAP://srv1/dc=dom,dc=company,dc=com",ADS_SETTYPE_FULL
set y = x.CopyPath
MsgBox y.Retrieve(ADS_FORMAT_WINDOWS)
```


The following VBScript/ASP code example shows how to make a copy of a pathname.


```vb
<%
Dim x, y
Const ADS_SETTYPE_FULL = 1
Const ADS_FORMAT_WINDOWS = 1
Set x = CreateObject("Pathname")
x.Set "LDAP://srv1/dc=dom,dc=company,dc=com",ADS_SETTYPE_FULL
 
set y = x.CopyPath
Response.Write y.Retrieve(ADS_FORMAT_WINDOWS)
%>
```


The following C++ code example creates a copy of a pathname object. For more information and a code example 
     of the <b>GetPathnameObject</b> function, see 
     <a href="https://msdn.microsoft.com/9aa26d6c-aa86-4a23-a986-b8cb9057772a">IADsPathname</a>.


```cpp
IADsPathname *pPath;
LPWSTR adsPath;
adsPath = L"LDAP://server/cn=jeff smith,dc=Fabrikam,dc=com";
 
IADsPathname *pPath = GetPathnameObject(adsPath)
if (!pPath) exit(0);
 
IDispatch *pDisp;
HRESULT hr;
hr = pPath->CopyPath(&pDisp);
if(FAILED(hr)) exit(hr);
 
IADsPathname *pPathCopy;
hr = pDisp->QueryInterface(IID_IADsPathname,(void**)&pPathCopy);
 
// ...
```





## -see-also




<a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>



<a href="https://msdn.microsoft.com/9aa26d6c-aa86-4a23-a986-b8cb9057772a">IADsPathname</a>
 

 

