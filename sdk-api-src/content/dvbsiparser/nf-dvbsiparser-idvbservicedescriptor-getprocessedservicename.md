---
UID: NF:dvbsiparser.IDvbServiceDescriptor.GetProcessedServiceName
title: IDvbServiceDescriptor::GetProcessedServiceName
author: windows-sdk-content
description: Gets the processed service name from a Digital Video Broadcast (DVB) service descriptor.
old-location: mstv\idvbservicedescriptor_getprocessedservicename.htm
tech.root: mstv
ms.assetid: c0441e70-270e-4685-9107-865c2b6398e9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetProcessedServiceName, GetProcessedServiceName method [Microsoft TV Technologies], GetProcessedServiceName method [Microsoft TV Technologies],IDvbServiceDescriptor interface, IDvbServiceDescriptor interface [Microsoft TV Technologies],GetProcessedServiceName method, IDvbServiceDescriptor.GetProcessedServiceName, IDvbServiceDescriptor::GetProcessedServiceName, dvbsiparser/IDvbServiceDescriptor::GetProcessedServiceName, mstv.idvbservicedescriptor_getprocessedservicename
ms.topic: method
req.header: dvbsiparser.h
req.include-header: Dvbsiparser.idl
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
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
 - dvbsiparser.h
api_name:
 - IDvbServiceDescriptor.GetProcessedServiceName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDvbServiceDescriptor::GetProcessedServiceName


## -description


 Gets the processed service name from a Digital Video Broadcast (DVB) service descriptor. 


## -parameters




### -param pbstrName [out]

Pointer to a buffer that receives the service name. The caller is responsible for freeing this memory.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This method calls <a href="https://msdn.microsoft.com/05d826fd-2795-4335-9f6f-f8e19a6dbe4c">IDvbServiceDescriptor2::GetServiceNameW</a> to get the processed  service name. It is provided to maintain compatibility with  the original DVB service descriptor specification.




## -see-also




<a href="https://msdn.microsoft.com/7024259f-3dcf-46e0-9984-d5924c9e5b54">IDvbServiceDescriptor</a>



<a href="https://msdn.microsoft.com/05d826fd-2795-4335-9f6f-f8e19a6dbe4c">IDvbServiceDescriptor2::GetServiceNameW</a>
 

 

