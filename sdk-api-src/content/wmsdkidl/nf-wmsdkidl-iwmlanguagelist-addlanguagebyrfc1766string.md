---
UID: NF:wmsdkidl.IWMLanguageList.AddLanguageByRFC1766String
title: IWMLanguageList::AddLanguageByRFC1766String
author: windows-sdk-content
description: The AddLanguageByRFC1766String method adds an entry to the list of supported languages for a file based upon a language tag compliant with RFC 1766.
old-location: wmformat\iwmlanguagelist_addlanguagebyrfc1766string.htm
tech.root: wmformat
ms.assetid: 3aec575c-8e04-4252-8863-1a458e56dcef
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddLanguageByRFC1766String, AddLanguageByRFC1766String method [windows Media Format], AddLanguageByRFC1766String method [windows Media Format],IWMLanguageList interface, IWMLanguageList interface [windows Media Format],AddLanguageByRFC1766String method, IWMLanguageList.AddLanguageByRFC1766String, IWMLanguageList::AddLanguageByRFC1766String, IWMLanguageListAddLanguageByRFC1766String, wmformat.iwmlanguagelist_addlanguagebyrfc1766string, wmsdkidl/IWMLanguageList::AddLanguageByRFC1766String
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wmvcore.lib
 - Wmvcore.dll
 - WMStubDRM.lib
 - WMStubDRM.dll
api_name:
 - IWMLanguageList.AddLanguageByRFC1766String
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMLanguageList::AddLanguageByRFC1766String


## -description



The <b>AddLanguageByRFC1766String</b> method adds an entry to the list of supported languages for a file based upon a language tag compliant with RFC 1766.




## -parameters




### -param pwszLanguageString [in]

Pointer to a wide-character null-terminated string containing an RFC 1766-compliant language tag.


### -param pwIndex [out]

Pointer to a <b>WORD</b>. On output, this will be set to the index assigned to the added language entry.


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
</table>
 




## -remarks



For a list of common RFC 1766-compliant language identifiers, see <a href="https://msdn.microsoft.com/625f7e95-0d21-4e16-8323-0f6301a04b30">Language Strings</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd757214(v=VS.85).aspx">IWMLanguageList Interface</a>
 

 

