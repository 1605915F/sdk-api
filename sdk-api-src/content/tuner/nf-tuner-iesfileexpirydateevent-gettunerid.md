---
UID: NF:tuner.IESFileExpiryDateEvent.GetTunerId
title: IESFileExpiryDateEvent::GetTunerId
author: windows-sdk-content
description: Gets a globally unique identifier (GUID) from a FileExpiryDate event that identifies the media transform device (MTD) that originated the event.
old-location: mstv\iesfileexpirydateevent_gettunerid.htm
tech.root: mstv
ms.assetid: 1271df60-7830-4e10-9af8-caf59aff56f8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetTunerId, GetTunerId method [Microsoft TV Technologies], GetTunerId method [Microsoft TV Technologies],IESFileExpiryDateEvent interface, IESFileExpiryDateEvent interface [Microsoft TV Technologies],GetTunerId method, IESFileExpiryDateEvent.GetTunerId, IESFileExpiryDateEvent::GetTunerId, mstv.iesfileexpirydateevent_gettunerid, tuner/IESFileExpiryDateEvent::GetTunerId
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
 - tuner.h
api_name:
 - IESFileExpiryDateEvent.GetTunerId
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IESFileExpiryDateEvent::GetTunerId


## -description


Gets a  globally unique identifier (GUID) from a <b>FileExpiryDate</b> event that identifies the media transform device (MTD) that originated the event.


## -parameters




### -param pguidTunerId [out, retval]

Receives the GUID for the MTD.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/6c89a3ee-7d69-4cde-b1e5-b566fa1c2ca3">IESFileExpiryDateEvent</a>
 

 

