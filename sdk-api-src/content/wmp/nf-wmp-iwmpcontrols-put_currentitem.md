---
UID: NF:wmp.IWMPControls.put_currentItem
title: IWMPControls::put_currentItem (wmp.h)
author: windows-sdk-content
description: The put_currentItem method specifies the current media item.
old-location: wmp\iwmpcontrols_put_currentitem.htm
tech.root: WMP
ms.assetid: 190cec53-5cd9-4bd0-b8d9-23c5389fe231
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWMPControls interface [Windows Media Player],put_currentItem method, IWMPControls.put_currentItem, IWMPControls::put_currentItem, IWMPControlsput_currentItem, put_currentItem, put_currentItem method [Windows Media Player], put_currentItem method [Windows Media Player],IWMPControls interface, wmp.iwmpcontrols_put_currentitem, wmp/IWMPControls::put_currentItem
ms.topic: method
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 9 Series or later.
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
req.lib: 
req.dll: Wmp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmp.dll
api_name:
 - IWMPControls.put_currentItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPControls::put_currentItem


## -description



The <b>put_currentItem</b> method specifies the current media item.




## -parameters




### -param pIWMPMedia [in]

Pointer to an <b>IWMPMedia</b> interface.


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



This method works only with items in the playlist. Calling <b>put_currentItem</b> with a reference to a saved media item is not supported.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd563179(v=VS.85).aspx">IWMPControls Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563197(v=VS.85).aspx">IWMPControls::get_currentItem</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563397(v=VS.85).aspx">IWMPMedia Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563554(v=VS.85).aspx">IWMPPlaylistCollection::getByName</a>
 

 

