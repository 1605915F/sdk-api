---
UID: NF:pla.IDataCollector.put_LatestOutputLocation
title: IDataCollector::put_LatestOutputLocation (pla.h)
author: windows-sdk-content
description: Retrieves or sets the fully decorated file name that PLA used the last time it created the file.
old-location: pla\idatacollector_latestoutputlocation.htm
tech.root: PLA
ms.assetid: e451c3a7-aec3-4fa7-9313-730bfac55f19
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IDataCollector interface [PLA],LatestOutputLocation property, IDataCollector.LatestOutputLocation, IDataCollector.put_LatestOutputLocation, IDataCollector::LatestOutputLocation, IDataCollector::get_LatestOutputLocation, IDataCollector::put_LatestOutputLocation, LatestOutputLocation property [PLA], LatestOutputLocation property [PLA],IDataCollector interface, base.idatacollector_latestoutputlocation, pla.idatacollector_latestoutputlocation, pla/IDataCollector::LatestOutputLocation, pla/IDataCollector::get_LatestOutputLocation, pla/IDataCollector::put_LatestOutputLocation, put_LatestOutputLocation
ms.topic: method
req.header: pla.h
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
req.lib: 
req.dll: Pla.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Pla.dll
api_name:
 - IDataCollector.LatestOutputLocation
 - IDataCollector.get_LatestOutputLocation
 - IDataCollector.put_LatestOutputLocation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDataCollector::put_LatestOutputLocation


## -description


Retrieves or sets the fully decorated file name that PLA used the last time it created the file.

This property is read/write.


## -parameters


## -remarks



Typically, you do not set this property. When the data collector starts, PLA sets this property using the value from the <a href="https://msdn.microsoft.com/c5453d16-4aa4-4c25-bfc7-514693317473">IDataCollector::OutputLocation</a> property.

You can set this property to empty if the file has been deleted.

For trace data collectors only, you can set this property to the name of the file to use. If it is not set, PLA creates it as it would for any other data collector.




## -see-also




<a href="https://msdn.microsoft.com/e1860bcf-c62d-434b-b98b-38bad7f84d89">IDataCollector</a>



<a href="https://msdn.microsoft.com/c5453d16-4aa4-4c25-bfc7-514693317473">IDataCollector::OutputLocation</a>
 

 

