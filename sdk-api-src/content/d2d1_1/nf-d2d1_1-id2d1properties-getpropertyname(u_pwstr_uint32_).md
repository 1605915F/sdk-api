---
UID: NF:d2d1_1.ID2D1Properties.GetPropertyName(U,PWSTR,UINT32,)
title: ID2D1Properties::GetPropertyName(U,PWSTR,UINT32,)
author: windows-sdk-content
description: Gets the property name that corresponds to the given index. This is a template overload. See Remarks.
old-location: direct2d\id2d1properties_getpropertyname2.htm
tech.root: Direct2D
ms.assetid: 777BF543-F2AF-4B17-BF2B-845D713EA5CA
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPropertyName, GetPropertyName method [Direct2D], GetPropertyName method [Direct2D],ID2D1Properties interface, ID2D1Properties interface [Direct2D],GetPropertyName method, ID2D1Properties.GetPropertyName, ID2D1Properties.GetPropertyName(U,PWSTR,UINT32,), ID2D1Properties::GetPropertyName, ID2D1Properties::GetPropertyName(U,PWSTR,UINT32), ID2D1Properties::GetPropertyName(U,PWSTR,UINT32,), d2d1_1/ID2D1Properties::GetPropertyName, direct2d.id2d1properties_getpropertyname2
ms.topic: method
req.header: d2d1_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D2d1.lib
req.dll: D2d1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D2d1.dll
api_name:
 - ID2D1Properties.GetPropertyName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1Properties::GetPropertyName(U,PWSTR,UINT32,)


## -description


Gets the property name that corresponds to the given index. This is a template overload. See Remarks.


## -parameters




### -param index

Type: <b>U</b>

The index of the property for which the name is being returned.


### -param name [out]

Type: <b>PWSTR</b>

When this method returns, contains the name being retrieved.


### -param nameCount

Type: <b>UINT32</b>

The number of characters in the <i>name</i> buffer.


### -param arg4

TBD




## -returns



Type: <b>HRESULT</b>

The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>HRESULT</th>
<th>Description</th>
</tr>
<tr>
<td>S_OK</td>
<td>No error occurred.</td>
</tr>
<tr>
<td>HRESULT_FROM_WIN32(ERROR_INSUFFICIENT_BUFFER)</td>
<td>The supplied buffer was too small to accomodate the data.</td>
</tr>
<tr>
<td>D2DERR_INVALID_PROPERTY</td>
<td>The specified property does not exist.</td>
</tr>
</table>
 




## -remarks



This method returns an empty string if <i>index</i> is invalid. If the method returns <b>RESULT_FROM_WIN32(ERROR_INSUFFICIENT_BUFFER)</b>, <i>name</i> will still be filled and truncated.


<pre class="syntax">template&lt;typename U&gt;
    HRESULT GetPropertyName(
        U index,
        _Out_writes_(nameCount) PWSTR name,
        UINT32 nameCount
        ) CONST;
</pre>





## -see-also




<a href="https://msdn.microsoft.com/7261ea3c-bd52-4809-93c8-9e7a0a7424d0">D2D1_PROPERTY</a>



<a href="https://msdn.microsoft.com/311a1b6f-ef0e-4453-a5fe-d06ebb0bb222">D2D1_SUBPROPERTY</a>



<a href="https://msdn.microsoft.com/dfe587f9-e92f-4367-a503-edd446a91cb8">ID2D1DeviceContext::CreateEffect</a>



<a href="https://msdn.microsoft.com/c38bfcc0-c696-41cc-9531-7c8f15c0b512">ID2D1Properties</a>
 

 

