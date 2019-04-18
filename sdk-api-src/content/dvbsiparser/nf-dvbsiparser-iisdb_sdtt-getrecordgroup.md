---
UID: NF:dvbsiparser.IISDB_SDTT.GetRecordGroup
title: IISDB_SDTT::GetRecordGroup (dvbsiparser.h)
author: windows-sdk-content
description: Receives the recording download level from a record in an Integrated services Digital Broadcasting (ISDB) software download trigger table (SDTT).
old-location: mstv\iisdb_sdtt_getrecordgroup.htm
tech.root: mstv
ms.assetid: 6798e477-754d-49a3-84f1-04d1a60094a7
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRecordGroup, GetRecordGroup method [Microsoft TV Technologies], GetRecordGroup method [Microsoft TV Technologies],IISDB_SDTT interface, IISDB_SDTT interface [Microsoft TV Technologies],GetRecordGroup method, IISDB_SDTT.GetRecordGroup, IISDB_SDTT::GetRecordGroup, dvbsiparser/IISDB_SDTT::GetRecordGroup, mstv.iisdb_sdtt_getrecordgroup
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
 - IISDB_SDTT.GetRecordGroup
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IISDB_SDTT::GetRecordGroup


## -description


Receives the recording download level from a record
  in an Integrated services Digital Broadcasting 
  (ISDB)  software download
  trigger table
  (SDTT). 


## -parameters




### -param dwRecordIndex [in]

Specifies the record number,
  indexed from zero. Call the <a href="https://msdn.microsoft.com/3e445eed-907c-4a9b-80b7-b16460bc131c">IISDB_SDTT::GetCountOfRecords</a>method to get the number of records in the SDTT.



### -param pbVal [out]

Receives the recording download level.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/f6ed35bc-4470-4000-8f0d-19d454453720">IISDB_SDTT</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd694352(v=VS.85).aspx">IISDB_SDTT::GetCountOfRecords</a>
 

 

