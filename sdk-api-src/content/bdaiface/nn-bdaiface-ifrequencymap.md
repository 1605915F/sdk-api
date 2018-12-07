---
UID: NN:bdaiface.IFrequencyMap
title: IFrequencyMap
author: windows-sdk-content
description: The IFrequencyMap interface sets the frequency table used by the BDA Network Provider filter.A frequency table is a list of broadcast or cable frequencies for a given country/region.
old-location: mstv\ifrequencymap.htm
tech.root: mstv
ms.assetid: 0f7f1b2c-a191-45f5-a645-367e898b6ee2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFrequencyMap, IFrequencyMap interface [Microsoft TV Technologies], IFrequencyMap interface [Microsoft TV Technologies],described, IFrequencyMapInterface, bdaiface/IFrequencyMap, mstv.ifrequencymap
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
 - IFrequencyMap
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFrequencyMap interface


## -description



The <b>IFrequencyMap</b> interface sets the frequency table used by the <a href="https://msdn.microsoft.com/en-us/library/Dd693014(v=VS.85).aspx">BDA Network Provider</a> filter.

A frequency table is a list of broadcast or cable frequencies for a given country/region. The Network Provider uses a frequency table to find the next frequency when <a href="https://msdn.microsoft.com/en-us/library/Dd694868(v=VS.85).aspx">IScanningTuner</a> methods are called. On startup, the Network Provider loads a default frequency table. An application can use the <b>IFrequencyMap</b> interface to specify the user's country/region, which causes the Network Provider filter to load the corresponding frequency table. The application can also modify the current table, or provide a completely new table, using the <a href="https://msdn.microsoft.com/en-us/library/Dd694092(v=VS.85).aspx">put_FrequencyMapping</a> method.

Frequencies used by this interface are measured in units of kilohertz (kHz), and refer to the center frequency of each band. For more information, see "Terrestrial delivery system descriptor" in the ETSI EN 300 468 standard.

<div class="alert"><b>Note</b>  Currently only the DVB-T Network Provider supports this interface.</div>
<div> </div>



## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFrequencyMap</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IFrequencyMap</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>IFrequencyMap</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694087(v=VS.85).aspx">get_CountryCode</a>
</td>
<td align="left" width="63%">
Returns the country/region code that the Network Provider is currently using.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694088(v=VS.85).aspx">get_CountryCodeList</a>
</td>
<td align="left" width="63%">
Returns a list of all the country/region codes for which the Network Provider has a frequency table.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694089(v=VS.85).aspx">get_DefaultFrequencyMapping</a>
</td>
<td align="left" width="63%">
Returns the default frequency table for a given country/region code.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694090(v=VS.85).aspx">get_FrequencyMapping</a>
</td>
<td align="left" width="63%">
Returns the Network Provider filter's current frequency table.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694091(v=VS.85).aspx">put_CountryCode</a>
</td>
<td align="left" width="63%">
Sets the country/region code.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd694092(v=VS.85).aspx">put_FrequencyMapping</a>
</td>
<td align="left" width="63%">
Sets the frequency table.

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IFrequencyMap)</code>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd693008(v=VS.85).aspx">BDA Interfaces</a>
 

 

