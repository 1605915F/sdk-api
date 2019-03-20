---
UID: NF:wmcontainer.IMFASFStreamSelector.GetOutputMutexCount
title: IMFASFStreamSelector::GetOutputMutexCount (wmcontainer.h)
author: windows-sdk-content
description: Retrieves the number of mutual exclusion objects associated with an output.
old-location: mf\imfasfstreamselector_getoutputmutexcount.htm
tech.root: medfound
ms.assetid: d6e98595-3307-47f5-806d-796350c78cec
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetOutputMutexCount, GetOutputMutexCount method [Media Foundation], GetOutputMutexCount method [Media Foundation],IMFASFStreamSelector interface, IMFASFStreamSelector interface [Media Foundation],GetOutputMutexCount method, IMFASFStreamSelector.GetOutputMutexCount, IMFASFStreamSelector::GetOutputMutexCount, d6e98595-3307-47f5-806d-796350c78cec, mf.imfasfstreamselector_getoutputmutexcount, wmcontainer/IMFASFStreamSelector::GetOutputMutexCount
ms.topic: method
req.header: wmcontainer.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfuuid.lib
 - mfuuid.dll
api_name:
 - IMFASFStreamSelector.GetOutputMutexCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFASFStreamSelector::GetOutputMutexCount


## -description



Retrieves the number of mutual exclusion objects associated with an output.




## -parameters




### -param dwOutputNum [in]

Output number for which to retrieve the count of mutually exclusive relationships.


### -param pcMutexes [out]

Receives the number of mutual exclusions.


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
 




## -see-also




<a href="https://msdn.microsoft.com/d2e1fc15-2e12-4698-a4b1-ca8046d228de">IMFASFStreamSelector</a>



<a href="https://msdn.microsoft.com/d134f4a9-9bca-454f-8dc1-2e152684a4bf">IMFASFStreamSelector::GetOutputMutex</a>
 

 

