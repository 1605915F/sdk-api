---
UID: NE:wmp.WMPBurnState
title: WMPBurnState (wmp.h)
author: windows-sdk-content
description: The WMPBurnState enumeration type defines the possible operational states of Windows Media Player as it burns a CD.
old-location: wmp\wmpburnstate.htm
tech.root: WMP
ms.assetid: fd286f68-4d36-48ae-800e-ad2be4c613c1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WMPBurnState, WMPBurnState enumeration [Windows Media Player], wmp.wmpburnstate, wmp/WMPBurnState, wmp/wmpbsBurning, wmp/wmpbsBusy, wmp/wmpbsErasing, wmp/wmpbsPreparingToBurn, wmp/wmpbsReady, wmp/wmpbsRefreshStatusPending, wmp/wmpbsStopped, wmp/wmpbsUnknown, wmp/wmpbsWaitingForDisc, wmpbsBurning, wmpbsBusy, wmpbsErasing, wmpbsPreparingToBurn, wmpbsReady, wmpbsRefreshStatusPending, wmpbsStopped, wmpbsUnknown, wmpbsWaitingForDisc
ms.topic: enum
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 11.
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - wmp.h
api_name:
 - WMPBurnState
product: Windows
targetos: Windows
req.typenames: WMPBurnState
req.redist: 
ms.custom: 19H1
---

# WMPBurnState enumeration


## -description



The <b>WMPBurnState</b> enumeration type defines the possible operational states of Windows Media Player as it burns a CD.




## -enum-fields




### -field wmpbsUnknown

Not a valid state.


### -field wmpbsBusy

Windows Media Player is busy. Try again in a moment.


### -field wmpbsReady

Ready to begin burning a CD.


### -field wmpbsWaitingForDisc

Waiting for the disc to become available.


### -field wmpbsRefreshStatusPending

The burn playlist has changed. Call <a href="https://msdn.microsoft.com/en-us/library/Dd563093(v=VS.85).aspx">IWMPCdromBurn::refreshStatus</a>.


### -field wmpbsPreparingToBurn

Windows Media Player is preparing to burn the CD.


### -field wmpbsBurning

The CD is being burned.


### -field wmpbsStopped

The burning operation is stopped.


### -field wmpbsErasing

Windows Media Player is erasing the CD.


### -field wmpbsDownloading




## -remarks



Windows Media Player 10 Mobile: This enumeration is not supported.




## -see-also




<a href="https://msdn.microsoft.com/90689fb7-656d-4c06-a0a9-02bbe0e5b5dd">Enumeration Types</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563081(v=VS.85).aspx">IWMPCdromBurn Interface</a>
 

 

