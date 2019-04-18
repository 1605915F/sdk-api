---
UID: NF:dvbsiparser.IPBDA_EIT.GetRecordDuration
title: IPBDA_EIT::GetRecordDuration (dvbsiparser.h)
author: windows-sdk-content
description: Gets the duration from an event record in an event information table (EIT) in a Protected Broadcast Device Architecture (PBDA) transport stream.
old-location: mstv\ipbda_eit_getrecordduration.htm
tech.root: mstv
ms.assetid: 898e211c-3228-441d-a099-907676da4bbe
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRecordDuration, GetRecordDuration method [Microsoft TV Technologies], GetRecordDuration method [Microsoft TV Technologies],IPBDA_EIT interface, IPBDA_EIT interface [Microsoft TV Technologies],GetRecordDuration method, IPBDA_EIT.GetRecordDuration, IPBDA_EIT::GetRecordDuration, dvbsiparser/IPBDA_EIT::GetRecordDuration, mstv.ipbda_eit_getrecordduration
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
 - IPBDA_EIT.GetRecordDuration
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPBDA_EIT::GetRecordDuration


## -description


 Gets the duration from an event record in an event information table (EIT) in a Protected Broadcast  Device Architecture (PBDA) transport stream.


## -parameters




### -param dwRecordIndex [in]

Specifies the service record number, indexed from zero.
  Call the <a href="https://msdn.microsoft.com/en-us/library/Dd694799(v=VS.85).aspx">IPBDA_EIT::GetCountOfRecords</a> method to get the number of records in the EIT.



### -param pmdVal [out]

Receives the event duration.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/cb8cd2cc-e498-43c2-ae1e-3543b4ea3b56">IPBDA_EIT</a>
 

 

