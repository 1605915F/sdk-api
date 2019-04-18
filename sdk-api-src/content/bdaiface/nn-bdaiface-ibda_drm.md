---
UID: NN:bdaiface.IBDA_DRM
title: IBDA_DRM (bdaiface.h)
author: windows-sdk-content
description: The IBDA_DRM interface is used to request a tuner to perform a DRM handshake with the user's computer.
old-location: mstv\ibda_drm.htm
tech.root: mstv
ms.assetid: d0bde207-d550-4e98-85c7-b0d47b0cd637
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IBDA_DRM, IBDA_DRM interface [Microsoft TV Technologies], IBDA_DRM interface [Microsoft TV Technologies],described, IBDA_DRMInterface, bdaiface/IBDA_DRM, mstv.ibda_drm
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
 - IBDA_DRM
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IBDA_DRM interface


## -description


The <b>IBDA_DRM</b> interface is used to request a tuner to perform a DRM handshake with the user's computer. Some tuners require a DRM handshake to verify that the user can receive content from the tuner. The BDA tuner filter exposes this interface; it is implemented by the tuner mini-driver.

<b>OCUR Devices: </b>This interface supports OpenCable Unidirectional Cable Receiver (OCUR) devices. See <a href="https://msdn.microsoft.com/7b641b94-9854-4ca8-8362-a9e1e49bbdd2">OCUR Devices</a>.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IBDA_DRM</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IBDA_DRM</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IBDA_DRM</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693319(v=VS.85).aspx">GetDRMPairingStatus</a>
</td>
<td align="left" width="63%">
Queries the status of the DRM handshake.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd693320(v=VS.85).aspx">PerformDRMPairing</a>
</td>
<td align="left" width="63%">
Requests the tuner to perform a DRM handshake.

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IBDA_DRM)</code>.




## -see-also




<a href="https://msdn.microsoft.com/07d18f73-e852-4c88-a2e2-e8f4198ca799">BDA Interfaces</a>
 

 

