---
UID: NF:dmort.MoFreeMediaType
title: MoFreeMediaType function (dmort.h)
author: windows-sdk-content
description: The MoFreeMediaType function frees the allocated members of a media type structure.
old-location: dshow\mofreemediatype.htm
tech.root: DirectShow
ms.assetid: a1f0949d-a590-4759-87b5-f47307bc3ec0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MoFreeMediaType, MoFreeMediaType function [DirectShow], dmort/MoFreeMediaType, dshow.mofreemediatype
ms.topic: function
req.header: dmort.h
req.include-header: Dmo.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Msdmo.lib
req.dll: Msdmo.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Msdmo.dll
api_name:
 - MoFreeMediaType
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MoFreeMediaType function


## -description


The <b>MoFreeMediaType</b> function frees the allocated members of a media type structure.


## -parameters




### -param pmt

Pointer to an initialized <a href="https://msdn.microsoft.com/en-us/library/Dd375504(v=VS.85).aspx">DMO_MEDIA_TYPE</a> structure.


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<b>NULL</b> pointer argument

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success

</td>
</tr>
</table>
 




## -remarks



Call this function to free a format block that was allocated with the <a href="https://msdn.microsoft.com/en-us/library/Dd390699(v=VS.85).aspx">MoInitMediaType</a> function. This function frees the <b>pbFormat</b> member of the <a href="https://msdn.microsoft.com/en-us/library/Dd375504(v=VS.85).aspx">DMO_MEDIA_TYPE</a> structure and sets <b>pbFormat</b> to <b>NULL</b>. The function does not reset the <b>cbFormat</b> member to zero, however, so if you re-use the <b>DMO_MEDIA_TYPE</b> structure, you should set <b>cbFormat</b> to zero.





