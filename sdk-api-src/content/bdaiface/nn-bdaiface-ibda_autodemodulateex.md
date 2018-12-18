---
UID: NN:bdaiface.IBDA_AutoDemodulateEx
title: IBDA_AutoDemodulateEx
author: windows-sdk-content
description: The IBDA_AutoDemodulateEx interface extends IBDA_AutoDemodulate.
old-location: mstv\ibda_autodemodulateex.htm
tech.root: mstv
ms.assetid: ecc642e4-7c36-400c-8a63-639f75b2bbc2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBDA_AutoDemodulateEx, IBDA_AutoDemodulateEx interface [Microsoft TV Technologies], IBDA_AutoDemodulateEx interface [Microsoft TV Technologies],described, IBDA_AutoDemodulateExInterface, bdaiface/IBDA_AutoDemodulateEx, mstv.ibda_autodemodulateex
ms.topic: interface
req.header: bdaiface.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: None supported
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Bdaiface.h
api_name:
 - IBDA_AutoDemodulateEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBDA_AutoDemodulateEx interface


## -description



The <b>IBDA_AutoDemodulateEx</b> interface extends <a href="https://msdn.microsoft.com/en-us/library/Dd693252(v=VS.85).aspx">IBDA_AutoDemodulate</a>. If a BDA device filter, specifically a demodulator, exposes this interface, it indicates that the filter can automatically detect signal characteristics. With this information, the Network Provider can be more efficient in managing the tuning process. For more information, see <b>KSPROPSETID_BdaAutodemodulate</b> in the Windows DDK.

<b>OCUR Devices: </b>This interface supports OpenCable Unidirectional Cable Receiver (OCUR) devices. See <a href="https://msdn.microsoft.com/7b641b94-9854-4ca8-8362-a9e1e49bbdd2">OCUR Devices</a>.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IBDA_AutoDemodulateEx</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Dd693252(v=VS.85).aspx">IBDA_AutoDemodulate</a>. <b>IBDA_AutoDemodulateEx</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IBDA_AutoDemodulateEx</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693254(v=VS.85).aspx">get_AuxInputCount</a>
</td>
<td align="left" width="63%">
Retrieves a count of the number of auxiliary inputs on the demodulator.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693255(v=VS.85).aspx">get_SupportedDeviceNodeTypes</a>
</td>
<td align="left" width="63%">
Retrieves a list of the device node types that the demodulator supports.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693256(v=VS.85).aspx">get_SupportedVideoFormats</a>
</td>
<td align="left" width="63%">
Retrieves the video formats that are supported by the demodulator.

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IBDA_AutoDemodulateEx)</code>.




## -see-also




<a href="https://msdn.microsoft.com/07d18f73-e852-4c88-a2e2-e8f4198ca799">BDA Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd693252(v=VS.85).aspx">IBDA_AutoDemodulate</a>
 

 

