---
UID: NF:dvbsiparser.IIsdbCADescriptor.GetPrivateDataBytes
title: IIsdbCADescriptor::GetPrivateDataBytes
author: windows-sdk-content
description: Gets the private data bytes from a conditional access (CA) descriptor.
old-location: mstv\iisdbcadescriptor_getprivatedatabytes.htm
tech.root: mstv
ms.assetid: cd64ba74-aab2-45eb-945a-187d3aaf9bdd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPrivateDataBytes, GetPrivateDataBytes method [Microsoft TV Technologies], GetPrivateDataBytes method [Microsoft TV Technologies],IIsdbCADescriptor interface, IIsdbCADescriptor interface [Microsoft TV Technologies],GetPrivateDataBytes method, IIsdbCADescriptor.GetPrivateDataBytes, IIsdbCADescriptor::GetPrivateDataBytes, dvbsiparser/IIsdbCADescriptor::GetPrivateDataBytes, mstv.iisdbcadescriptor_getprivatedatabytes
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dvbsiparser.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Dvbsiparser.idl
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
 - IIsdbCADescriptor.GetPrivateDataBytes
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IIsdbCADescriptor::GetPrivateDataBytes


## -description


Gets the private data bytes from a conditional access (CA) descriptor. 


## -parameters




### -param pbBufferLength [in, out]

On input, specifies the length of the private data being retrieved, in bytes. On output, returns the actual data length.


### -param pbBuffer [out]

Receives the conditional access private data.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/6683f3db-636b-42bb-a46d-c175a4324023">IIsdbCADescriptor</a>
 

 

