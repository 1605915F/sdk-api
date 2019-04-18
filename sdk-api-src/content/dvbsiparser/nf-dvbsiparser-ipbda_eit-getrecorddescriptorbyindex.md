---
UID: NF:dvbsiparser.IPBDA_EIT.GetRecordDescriptorByIndex
title: IPBDA_EIT::GetRecordDescriptorByIndex (dvbsiparser.h)
author: windows-sdk-content
description: Retrieves a descriptor for a specified record in an event information table (EIT) in a Protected Broadcast Device Architecture (PBDA) transport stream.
old-location: mstv\ipbda_eit_getrecorddescriptorbyindex.htm
tech.root: mstv
ms.assetid: 96ca5a6b-c515-4854-8e95-9cb155879b3b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRecordDescriptorByIndex, GetRecordDescriptorByIndex method [Microsoft TV Technologies], GetRecordDescriptorByIndex method [Microsoft TV Technologies],IPBDA_EIT interface, IPBDA_EIT interface [Microsoft TV Technologies],GetRecordDescriptorByIndex method, IPBDA_EIT.GetRecordDescriptorByIndex, IPBDA_EIT::GetRecordDescriptorByIndex, dvbsiparser/IPBDA_EIT::GetRecordDescriptorByIndex, mstv.ipbda_eit_getrecorddescriptorbyindex
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
 - IPBDA_EIT.GetRecordDescriptorByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPBDA_EIT::GetRecordDescriptorByIndex


## -description


 Retrieves a descriptor for a specified record in an  event information table (EIT) in a Protected Broadcast  Device Architecture (PBDA) transport stream.


## -parameters




### -param dwRecordIndex [in]

Specifies the service record number, indexed from zero.
  Call the <a href="https://msdn.microsoft.com/en-us/library/Dd694799(v=VS.85).aspx">IPBDA_EIT::GetCountOfRecords</a> method to get the number of records in the EIT.



### -param dwIndex [in]

Specifies the descriptor to retrieve, indexed from zero. Call the <a href="https://msdn.microsoft.com/c491b2d0-6426-4a76-b3a1-4477fdf1779c">IPBDA_EIT::GetRecordCountOfDescriptors</a> method to get the number of descriptors for a particular record.


### -param ppDescriptor [out]

Address of a variable that receives an <a href="https://msdn.microsoft.com/en-us/library/Dd694093(v=VS.85).aspx">IGenericDescriptor</a> interface pointer. Use this interface to retrieve the information in the descriptor. The caller must release the interface.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd694093(v=VS.85).aspx">IGenericDescriptor</a>



<a href="https://msdn.microsoft.com/cb8cd2cc-e498-43c2-ae1e-3543b4ea3b56">IPBDA_EIT</a>
 

 

