---
UID: NF:wmp.IWMPControls2.step
title: IWMPControls2::step
author: windows-sdk-content
description: The step method causes the current video media item to freeze playback on the next frame or the previous frame.
old-location: wmp\iwmpcontrols2_step.htm
tech.root: WMP
ms.assetid: d54a4bb7-855f-4807-89b5-176b7fac2edd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPControls2 interface [Windows Media Player],step method, IWMPControls2.step, IWMPControls2::step, IWMPControls2step, step, step method [Windows Media Player], step method [Windows Media Player],IWMPControls2 interface, wmp.iwmpcontrols2_step, wmp/IWMPControls2::step
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IWMPControls2.step
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPControls2::step


## -description



The <b>step</b> method causes the current video media item to freeze playback on the next frame or the previous frame.




## -parameters




### -param lStep [in]

<b>long</b> indicating how many frames to step before freezing. Must be set to 1 or -1.


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



This method currently only supports the parameters 1 or -1, so you can only step one frame at a time.

<b>Windows Media Player 10 Mobile: </b>This method always returns E_INVALIDARG.




## -see-also




<a href="https://msdn.microsoft.com/aadbd924-b583-4136-8d6c-e3c8c0b3872e">IWMPControls2 Interface</a>



<a href="https://msdn.microsoft.com/d133f1e1-cbeb-403d-b247-9f495cb6f0f7">IWMPDVD Interface</a>
 

 

