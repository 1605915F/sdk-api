---
UID: NF:dvbsiparser.IISDB_SDTT.GetRecordCountOfSchedules
title: IISDB_SDTT::GetRecordCountOfSchedules (dvbsiparser.h)
author: windows-sdk-content
description: Returns the number of schedules from a record in an Information for Digital Broadcasting System (IDBS) software download trigger table (SDTT).
old-location: mstv\iisdb_sdtt_getrecordcountofschedules.htm
tech.root: mstv
ms.assetid: c8f757de-779c-43df-9f24-caf527e91f03
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRecordCountOfSchedules, GetRecordCountOfSchedules method [Microsoft TV Technologies], GetRecordCountOfSchedules method [Microsoft TV Technologies],IISDB_SDTT interface, IISDB_SDTT interface [Microsoft TV Technologies],GetRecordCountOfSchedules method, IISDB_SDTT.GetRecordCountOfSchedules, IISDB_SDTT::GetRecordCountOfSchedules, dvbsiparser/IISDB_SDTT::GetRecordCountOfSchedules, mstv.iisdb_sdtt_getrecordcountofschedules
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
 - IISDB_SDTT.GetRecordCountOfSchedules
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IISDB_SDTT::GetRecordCountOfSchedules


## -description


Returns the number of schedules from a
  record in an Information for Digital Broadcasting System
  (IDBS)  software download
  trigger table
  (SDTT). 


## -parameters




### -param dwRecordIndex [in]

Specifies the record number, indexed from zero.
  Call the <a href="https://msdn.microsoft.com/3e445eed-907c-4a9b-80b7-b16460bc131c">IISDB_SDTT::GetCountOfRecords</a> method to get the number of records in the SDTT.



### -param pdwVal [out]

Receives the number of schedules.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/f6ed35bc-4470-4000-8f0d-19d454453720">IISDB_SDTT</a>



<a href="https://msdn.microsoft.com/3e445eed-907c-4a9b-80b7-b16460bc131c">IISDB_SDTT::GetCountOfRecords</a>
 

 

