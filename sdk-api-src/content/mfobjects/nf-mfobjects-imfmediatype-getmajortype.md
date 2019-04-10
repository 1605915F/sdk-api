---
UID: NF:mfobjects.IMFMediaType.GetMajorType
title: IMFMediaType::GetMajorType (mfobjects.h)
author: windows-sdk-content
description: Gets the major type of the format.
old-location: mf\imfmediatype_getmajortype.htm
tech.root: medfound
ms.assetid: 98f0a9ca-4766-4d2b-89b8-d6e30b75f47d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 98f0a9ca-4766-4d2b-89b8-d6e30b75f47d, GetMajorType, GetMajorType method [Media Foundation], GetMajorType method [Media Foundation],IMFMediaType interface, IMFMediaType interface [Media Foundation],GetMajorType method, IMFMediaType.GetMajorType, IMFMediaType::GetMajorType, mf.imfmediatype_getmajortype, mfobjects/IMFMediaType::GetMajorType
ms.topic: method
req.header: mfobjects.h
req.include-header: Mfidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfuuid.lib
 - mfuuid.dll
api_name:
 - IMFMediaType.GetMajorType
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFMediaType::GetMajorType


## -description


Gets the major type of the format.
        


## -parameters




### -param pguidMajorType [out]

Receives the major type <b>GUID</b>. The major type describes the broad category of the format, such as audio or video. For a list of possible values, see <a href="https://msdn.microsoft.com/1cca3539-a920-4938-93b9-ae41e1c0a287">Major Media Types</a>.
          


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.
          

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.
              

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MF_E_ATTRIBUTENOTFOUND</b></dt>
</dl>
</td>
<td width="60%">
The major type is not set.
              

</td>
</tr>
</table>
 




## -remarks



This method is equivalent to getting the <a href="https://msdn.microsoft.com/b88b5fcf-8025-4638-930d-9fc5cf0ec8a3">MF_MT_MAJOR_TYPE</a> attribute from the media type.
      

This interface is available on the following platforms if the Windows Media Format 11 SDK redistributable components are installed:

<ul>
<li>Windows XP with Service Pack 2 (SP2) and later.</li>
<li>Windows XP Media Center Edition 2005 with KB900325 (Windows XP Media Center Edition 2005) and KB925766 (October 2006 Update Rollup for Windows XP Media Center Edition) installed.</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/f1d60bec-71e4-4fcc-a020-92754b6f3c02">IMFMediaType</a>
 

 

