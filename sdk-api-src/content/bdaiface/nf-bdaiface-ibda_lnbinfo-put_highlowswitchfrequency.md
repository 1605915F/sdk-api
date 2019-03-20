---
UID: NF:bdaiface.IBDA_LNBInfo.put_HighLowSwitchFrequency
title: IBDA_LNBInfo::put_HighLowSwitchFrequency (bdaiface.h)
author: windows-sdk-content
description: The put_HighLowSwitchFrequency method specifies the frequency of the high-low switch.
old-location: mstv\ibda_lnbinfo_put_highlowswitchfrequency.htm
tech.root: mstv
ms.assetid: 3edde05f-1cdb-4648-a34b-ba95e4fcff12
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBDA_LNBInfo interface [Microsoft TV Technologies],put_HighLowSwitchFrequency method, IBDA_LNBInfo.put_HighLowSwitchFrequency, IBDA_LNBInfo::put_HighLowSwitchFrequency, IBDA_LNBInfoput_HighLowSwitchFrequency, bdaiface/IBDA_LNBInfo::put_HighLowSwitchFrequency, mstv.ibda_lnbinfo_put_highlowswitchfrequency, put_HighLowSwitchFrequency, put_HighLowSwitchFrequency method [Microsoft TV Technologies], put_HighLowSwitchFrequency method [Microsoft TV Technologies],IBDA_LNBInfo interface
ms.topic: method
req.header: bdaiface.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
 - COM
api_location:
 - bdaiface.h
api_name:
 - IBDA_LNBInfo.put_HighLowSwitchFrequency
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBDA_LNBInfo::put_HighLowSwitchFrequency


## -description



The <b>put_HighLowSwitchFrequency</b> method specifies the frequency of the high-low switch.




## -parameters




### -param ulSwitchFrequency [in]

Specifies the frequency. The units are 1 Hz x the frequency multiplier, where the <i>frequency multiplier</i> is the value returned by the <a href="https://msdn.microsoft.com/en-us/library/Dd693359(v=VS.85).aspx">IBDA_FrequencyFilter::get_FrequencyMultiplier</a> method. The default frequency multiplier is 1000, so the default units are kilohertz (kHz).


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd693396(v=VS.85).aspx">IBDA_LNBInfo Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd693397(v=VS.85).aspx">IBDA_LNBInfo::get_HighLowSwitchFrequency</a>
 

 

