---
UID: NF:bdaiface.IBDA_ConditionalAccessEx.OpenBroadcastMmi
title: IBDA_ConditionalAccessEx::OpenBroadcastMmi
author: windows-sdk-content
description: Responds to a BroadcastMMI event.
old-location: mstv\ibda_conditionalaccessex_openbroadcastmmi.htm
tech.root: mstv
ms.assetid: 15390805-ff09-4dca-b00d-ad2f3641911b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBDA_ConditionalAccessEx interface [Microsoft TV Technologies],OpenBroadcastMmi method, IBDA_ConditionalAccessEx.OpenBroadcastMmi, IBDA_ConditionalAccessEx::OpenBroadcastMmi, OpenBroadcastMmi, OpenBroadcastMmi method [Microsoft TV Technologies], OpenBroadcastMmi method [Microsoft TV Technologies],IBDA_ConditionalAccessEx interface, bdaiface/IBDA_ConditionalAccessEx::OpenBroadcastMmi, mstv.ibda_conditionalaccessex_openbroadcastmmi
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: bdaiface.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bdaiface.idl
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
 - bdaiface.h
api_name:
 - IBDA_ConditionalAccessEx.OpenBroadcastMmi
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBDA_ConditionalAccessEx::OpenBroadcastMmi


## -description


Responds to a BroadcastMMI event.

When a device receives a BroadcastMMI event, it calls this method one time for each user interface (MMI) dialog box that is displayed to the user. 


## -parameters




### -param ulDialogRequest [in]

A logical link with the MMI dialog box that was triggered by the action.


### -param bstrLanguage [in]

The language of the dialog box. This string contains an ISO 639-2 language code with a dash followed by an ISO 3166 country/region code.


### -param EventId [in]

The event identifier of the BroadcastMMI event.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd693262(v=VS.85).aspx">IBDA_ConditionalAccessEx</a>
 

 

