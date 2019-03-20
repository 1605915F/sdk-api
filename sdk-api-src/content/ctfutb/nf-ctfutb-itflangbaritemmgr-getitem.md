---
UID: NF:ctfutb.ITfLangBarItemMgr.GetItem
title: ITfLangBarItemMgr::GetItem (ctfutb.h)
author: windows-sdk-content
description: ITfLangBarItemMgr::GetItem method
old-location: tsf\itflangbaritemmgr_getitem.htm
tech.root: TSF
ms.assetid: 35895fd7-23d0-416b-98c2-45192edf0a6b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetItem, GetItem method [Text Services Framework], GetItem method [Text Services Framework],ITfLangBarItemMgr interface, ITfLangBarItemMgr interface [Text Services Framework],GetItem method, ITfLangBarItemMgr.GetItem, ITfLangBarItemMgr::GetItem, _tsf_itflangbaritemmgr_getitem_ref, ctfutb/ITfLangBarItemMgr::GetItem, tsf.itflangbaritemmgr_getitem
ms.topic: method
req.header: ctfutb.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Ctfutb.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Msctf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - msctf.dll
api_name:
 - ITfLangBarItemMgr.GetItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfLangBarItemMgr::GetItem


## -description




## -parameters




### -param rguid [in]

GUID that identifies the item to obtain. This is the item GUID that the item supplies in <a href="https://msdn.microsoft.com/b32e433a-c0d6-418e-bf11-2291c85373c2">ITfLangBarItem::GetInfo</a>. This identifier can be a custom value or one of the <a href="https://msdn.microsoft.com/6280cde9-2350-48a9-8740-01a856b0a1bc">predefined language bar items</a>.


### -param ppItem [out]

Pointer to an <a href="https://msdn.microsoft.com/16612641-2bff-4e6f-a955-85793021a20b">ITfLangBarItem</a> interface pointer that receives the item interface.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The item cannot be found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppItem</i> parameter is invalid.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/16612641-2bff-4e6f-a955-85793021a20b">ITfLangBarItem</a>



<a href="https://msdn.microsoft.com/b32e433a-c0d6-418e-bf11-2291c85373c2">ITfLangBarItem::GetInfo</a>



<a href="https://msdn.microsoft.com/a7fa257f-e600-4554-8b23-f73323f37e69">ITfLangBarItemMgr</a>



<a href="https://msdn.microsoft.com/6280cde9-2350-48a9-8740-01a856b0a1bc">Predefined language bar items
      </a>
 

 

