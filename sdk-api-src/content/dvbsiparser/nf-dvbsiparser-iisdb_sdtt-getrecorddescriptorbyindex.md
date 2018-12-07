---
UID: NF:dvbsiparser.IISDB_SDTT.GetRecordDescriptorByIndex
title: IISDB_SDTT::GetRecordDescriptorByIndex
author: windows-sdk-content
description: Returns a descriptor for a specified record in an Integrated Services Digital Broadcasting (ISDB) software download trigger table (SDTT).
old-location: mstv\iisdb_sdtt_getrecorddescriptorbyindex.htm
tech.root: mstv
ms.assetid: c8aab681-4858-4ad2-84a7-15a9b8310d6f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetRecordDescriptorByIndex, GetRecordDescriptorByIndex method [Microsoft TV Technologies], GetRecordDescriptorByIndex method [Microsoft TV Technologies],IISDB_SDTT interface, IISDB_SDTT interface [Microsoft TV Technologies],GetRecordDescriptorByIndex method, IISDB_SDTT.GetRecordDescriptorByIndex, IISDB_SDTT::GetRecordDescriptorByIndex, dvbsiparser/IISDB_SDTT::GetRecordDescriptorByIndex, mstv.iisdb_sdtt_getrecorddescriptorbyindex
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IISDB_SDTT.GetRecordDescriptorByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IISDB_SDTT::GetRecordDescriptorByIndex


## -description


Returns a descriptor for a specified record
  in an Integrated Services Digital Broadcasting (ISDB) software download
  trigger table
  (SDTT).


## -parameters




### -param dwRecordIndex [in]

Specifies the record number, indexed from zero.
  Call the <a href="https://msdn.microsoft.com/3e445eed-907c-4a9b-80b7-b16460bc131c">IISDB_SDTT::GetCountOfRecords</a> method to get the number
  of records in the SDTT.



### -param dwIndex [in]

Specifies which descriptor to retrieve, indexed from zero.
  Call the <a href="https://msdn.microsoft.com/04f32111-4c4b-4f5b-81d1-fa7c19841cd8">IISDB_SDTT::GetRecordCountOfDescriptors</a> method to get the number
  of descriptors for a particular record.



### -param ppDescriptor [out]

Pointer to the <a href="https://msdn.microsoft.com/efca0ecf-eb3e-4dcd-a674-b8fe1a66ff84">IGenericDescriptor</a> interface for the descriptor being retrieved. The caller is responsible for freeing this memory.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/efca0ecf-eb3e-4dcd-a674-b8fe1a66ff84">IGenericDescriptor</a>



<a href="https://msdn.microsoft.com/f6ed35bc-4470-4000-8f0d-19d454453720">IISDB_SDTT</a>



<a href="https://msdn.microsoft.com/3e445eed-907c-4a9b-80b7-b16460bc131c">IISDB_SDTT::GetCountOfRecords</a>



<a href="https://msdn.microsoft.com/04f32111-4c4b-4f5b-81d1-fa7c19841cd8">IISDB_SDTT::GetRecordCountOfDescriptors</a>
 

 

