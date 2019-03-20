---
UID: NF:adshlp.ADsFreeEnumerator
title: ADsFreeEnumerator function (adshlp.h)
author: windows-sdk-content
description: Frees an enumerator object created with the ADsBuildEnumerator function.
old-location: adsi\adsfreeenumerator.htm
tech.root: adsi
ms.assetid: 0ac13320-c0c2-45e3-b1c0-b4bf6c7e5315
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ADsFreeEnumerator, ADsFreeEnumerator function [ADSI], _ds_adsfreeenumerator, adshlp/ADsFreeEnumerator, adsi.adsfreeenumerator
ms.topic: function
req.header: adshlp.h
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
req.lib: Activeds.lib
req.dll: Activeds.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Activeds.dll
api_name:
 - ADsFreeEnumerator
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ADsFreeEnumerator function


## -description


The <b>ADsFreeEnumerator</b> function frees an enumerator object created with the  <a href="https://msdn.microsoft.com/e4fdec19-bccf-49ec-8a95-29e096c4c9c1">ADsBuildEnumerator</a> function.


## -parameters




### -param pEnumVariant [in]

Type: <b>IEnumVARIANT*</b>

Pointer to the  <a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a> interface on the enumerator object to be freed.


## -returns



Type: <b>HRESULT</b>

This method supports standard return values, as well as the following.




## -remarks



The general process for enumerating objects in a container is as follows.

First, create an enumerator object on that container.

Second, retrieve the <a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a> interface pointer.

Third, call the <a href="https://msdn.microsoft.com/9bfc98a5-f4f0-4127-89c9-b8ed01bfde4e">ADsEnumerateNext</a> function to return an enumerated set of elements from the enumerator object.

Fourth, call the <b>ADSFreeEnumerator</b> function to free the enumerator object.

For more information and a code example, see <a href="https://msdn.microsoft.com/e4fdec19-bccf-49ec-8a95-29e096c4c9c1">ADsBuildEnumerator</a>.




## -see-also




<a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>



<a href="https://msdn.microsoft.com/4f0e90e2-afcc-4cf7-a731-9b38a83ca229">ADSI Functions</a>



<a href="https://msdn.microsoft.com/e4fdec19-bccf-49ec-8a95-29e096c4c9c1">ADsBuildEnumerator</a>



<a href="https://msdn.microsoft.com/9bfc98a5-f4f0-4127-89c9-b8ed01bfde4e">ADsEnumerateNext</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a>
 

 

