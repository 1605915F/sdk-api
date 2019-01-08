---
UID: NF:pla.IDataCollectorSet.get_SerialNumber
title: IDataCollectorSet::get_SerialNumber
author: windows-sdk-content
description: Retrieves or sets the number of times that this data collector set has been started, including segments.
old-location: pla\idatacollectorset_get_serialnumber.htm
tech.root: PLA
ms.assetid: 92bfd307-362e-4d60-9a61-d2096fbb3d19
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDataCollectorSet interface [PLA],SerialNumber property, IDataCollectorSet.SerialNumber, IDataCollectorSet.get_SerialNumber, IDataCollectorSet::SerialNumber, IDataCollectorSet::get_SerialNumber, IDataCollectorSet::put_SerialNumber, SerialNumber property [PLA], SerialNumber property [PLA],IDataCollectorSet interface, base.idatacollectorset_get_serialnumber, get_SerialNumber, pla.idatacollectorset_get_serialnumber, pla/IDataCollectorSet::SerialNumber, pla/IDataCollectorSet::get_SerialNumber, pla/IDataCollectorSet::put_SerialNumber
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
 - IDataCollectorSet.SerialNumber
 - IDataCollectorSet.get_SerialNumber
 - IDataCollectorSet.put_SerialNumber
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDataCollectorSet::get_SerialNumber


## -description


Retrieves or sets the number of times that this data collector set has been started, including segments.

This property is read/write.


## -parameters


## -remarks



Use this property if the <a href="https://msdn.microsoft.com/f9e6eb88-ac38-4b99-ab64-a408f75f7969">IDataCollectorSet::SubdirectoryFormat</a> property is set to <b>plaSerialNumber</b>.

PLA increments the serial number after using it.




## -see-also




<a href="https://msdn.microsoft.com/a4ae0874-4ee6-46a1-9811-8cd4be26859c">IDataCollectorSet</a>
 

 

