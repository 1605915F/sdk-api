---
UID: NF:dvbsiparser.IISDB_NBIT.GetRecordDescriptorByIndex
title: IISDB_NBIT::GetRecordDescriptorByIndex (dvbsiparser.h)
author: windows-sdk-content
description: Retrieves a descriptor for a specified record in an Integrated Services Digital Broadcasting (ISDB) network broadcaster information table (NBIT) based on the descriptor index.
old-location: mstv\iisdb_nbit_getrecorddescriptorbyindex.htm
tech.root: mstv
ms.assetid: 0f7da95d-ba3f-4cdc-aea0-38abae260159
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRecordDescriptorByIndex, GetRecordDescriptorByIndex method [Microsoft TV Technologies], GetRecordDescriptorByIndex method [Microsoft TV Technologies],IISDB_NBIT interface, IISDB_NBIT interface [Microsoft TV Technologies],GetRecordDescriptorByIndex method, IISDB_NBIT.GetRecordDescriptorByIndex, IISDB_NBIT::GetRecordDescriptorByIndex, dvbsiparser/IISDB_NBIT::GetRecordDescriptorByIndex, mstv.iisdb_nbit_getrecorddescriptorbyindex
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
 - IISDB_NBIT.GetRecordDescriptorByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IISDB_NBIT::GetRecordDescriptorByIndex


## -description


Retrieves a descriptor for a specified record in 
  an Integrated Services Digital Broadcasting (ISDB) 
  network broadcaster information table (NBIT)
  based on the descriptor index.


## -parameters




### -param dwRecordIndex [in]

Specifies the record number, indexed from zero. 
Call the <a href="https://msdn.microsoft.com/c747278a-dea7-4772-b37d-89c1deaaf91f">IISDB_NBIT::GetCountOfRecords</a> 
 method to get the number 
of records in the NBIT.


### -param dwIndex [in]

Specifies which descriptor to retrieve, indexed from zero. 
Call the <a href="https://msdn.microsoft.com/2f4f5b5a-f03a-4b90-aa7c-2552841ba165">IISDB_NBIT::GetRecordCountOfDescriptors</a> method 
to get the number of descriptors for a particular record.


### -param ppDescriptor [out]

Pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd694093(v=VS.85).aspx">IGenericDescriptor</a> interface implemented by the descriptor. The caller is responsible for freeing the interface.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd694093(v=VS.85).aspx">IGenericDescriptor</a>



<a href="https://msdn.microsoft.com/32c15a03-6683-4b22-b374-a15784696368">IISDB_NBIT</a>



<a href="https://msdn.microsoft.com/2f4f5b5a-f03a-4b90-aa7c-2552841ba165">IISDB_NBIT::GetRecordCountOfDescriptors</a>
 

 

