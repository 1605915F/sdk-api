---
UID: NF:bdatif.IGuideData.GetServices
title: IGuideData::GetServices
author: windows-sdk-content
description: The GetServices method retrieves a collection of tune requests representing all the services available in the tuning space.
old-location: mstv\iguidedata_getservices.htm
tech.root: mstv
ms.assetid: a3c08812-ed56-440e-a88d-80e20a681695
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetServices, GetServices method [Microsoft TV Technologies], GetServices method [Microsoft TV Technologies],IGuideData interface, IGuideData interface [Microsoft TV Technologies],GetServices method, IGuideData.GetServices, IGuideData::GetServices, IGuideDataGetServices, bdatif/IGuideData::GetServices, mstv.iguidedata_getservices
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: bdatif.h
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
 - bdatif.h
api_name:
 - IGuideData.GetServices
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IGuideData::GetServices


## -description



The <b>GetServices</b> method retrieves a collection of tune requests representing all the services available in the tuning space.




## -parameters




### -param ppEnumTuneRequests [out]

Pointer to a variable that receives an <a href="https://msdn.microsoft.com/en-us/library/Dd694005(v=VS.85).aspx">IEnumTuneRequests</a> interface pointer. Use this interface to enumerate the properties. The caller must release the interface.


## -returns



The method returns an <b>HRESULT</b>. Possible values include those in the following table.

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



This method is used to enumerate all services listed in the service descriptor table. Each tune request in the returned collection contains locator data for the service. To get more information about a service, pass the <a href="https://msdn.microsoft.com/en-us/library/Dd694997(v=VS.85).aspx">ITuneRequest</a> pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd694116(v=VS.85).aspx">IGuideData::GetServiceProperties</a> method.

The method fails if the TIF has not received the service information from the PSI tables in the transport stream. The client should implement the <a href="https://msdn.microsoft.com/en-us/library/Dd694099(v=VS.85).aspx">IGuideDataEvent</a> interface and wait for the <a href="https://msdn.microsoft.com/en-us/library/Dd694105(v=VS.85).aspx">IGuideDataEvent::ServiceChanged</a> event to be fired.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd375623(v=VS.85).aspx">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd694098(v=VS.85).aspx">IGuideData Interface</a>
 

 

