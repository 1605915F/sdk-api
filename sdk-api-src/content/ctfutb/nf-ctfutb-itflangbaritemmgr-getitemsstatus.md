---
UID: NF:ctfutb.ITfLangBarItemMgr.GetItemsStatus
title: ITfLangBarItemMgr::GetItemsStatus
author: windows-sdk-content
description: ITfLangBarItemMgr::GetItemsStatus method
old-location: tsf\itflangbaritemmgr_getitemsstatus.htm
tech.root: TSF
ms.assetid: bf0bbbd5-63ca-4f2e-afee-e0c47d6e3d7b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetItemsStatus, GetItemsStatus method [Text Services Framework], GetItemsStatus method [Text Services Framework],ITfLangBarItemMgr interface, ITfLangBarItemMgr interface [Text Services Framework],GetItemsStatus method, ITfLangBarItemMgr.GetItemsStatus, ITfLangBarItemMgr::GetItemsStatus, _tsf_itflangbaritemmgr_getitemsstatus_ref, ctfutb/ITfLangBarItemMgr::GetItemsStatus, tsf.itflangbaritemmgr_getitemsstatus
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ITfLangBarItemMgr.GetItemsStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
---

# ITfLangBarItemMgr::GetItemsStatus


## -description




## -parameters




### -param ulCount [in]

Specifies the number of items to obtain the status for.


### -param prgguid [in]

Pointer to an array of <b>GUID</b>s that identify the items obtain the status for. These are the item <b>GUID</b>s that the item supplies in <a href="https://msdn.microsoft.com/en-us/library/ms628741(v=VS.85).aspx">ITfLangBarItem::GetInfo</a>. This array must be at least <i>ulCount</i> elements in length.


### -param pdwStatus [out]

Pointer to an array of <b>DWORD</b> values that receive the status of each item. Each element in this array receives zero or a combination of one or more of the <a href="https://msdn.microsoft.com/en-us/library/ms629077(v=VS.85).aspx">TF_LBI_STATUS_*</a> values. This array must be at least <i>ulCount</i> elements in length.

The index of each status value cooresponds to the index of the item identifier in <i>prgguid</i>. For example, the element 0 in <i>pdwStatus</i> receives the for the item identified by element 0 of <i>prgguid</i>.


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
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unspecified error occurred.

</td>
</tr>
</table>
 




## -remarks



This method causes the <a href="https://msdn.microsoft.com/en-us/library/ms628743(v=VS.85).aspx">ITfLangBarItem::GetStatus</a> method of each language bar item identified by <i>prgguid</i> to be called.




## -see-also




<a href="https://msdn.microsoft.com/2f850553-ec79-4e2f-a4d5-c40dbaca0f01">ITfLangBarItem::GetStatus
      </a>



<a href="https://msdn.microsoft.com/en-us/library/ms628723(v=VS.85).aspx">ITfLangBarItemMgr</a>



<a href="https://msdn.microsoft.com/5f2c0e61-f7e5-4dcc-86a3-7bd1c994b8bc">TF_LBI_STATUS_* Constants
      </a>
 

 

