---
UID: NF:dvbsiparser.IDvbMultilingualServiceNameDescriptor.GetRecordLangId
title: IDvbMultilingualServiceNameDescriptor::GetRecordLangId
author: windows-sdk-content
description: Gets the three-character ISO 639 language code from a Digital Video Broadcast (DVB) multilingual service name descriptor. The language code identifies the language used for text in the descriptor.
old-location: mstv\idvbmultilingualservicenamedescriptor_getrecordlangid.htm
tech.root: mstv
ms.assetid: a8432acb-f59b-4995-8b5d-576acab0f6b1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetRecordLangId, GetRecordLangId method [Microsoft TV Technologies], GetRecordLangId method [Microsoft TV Technologies],IDvbMultilingualServiceNameDescriptor interface, IDvbMultilingualServiceNameDescriptor interface [Microsoft TV Technologies],GetRecordLangId method, IDvbMultilingualServiceNameDescriptor.GetRecordLangId, IDvbMultilingualServiceNameDescriptor::GetRecordLangId, dvbsiparser/IDvbMultilingualServiceNameDescriptor::GetRecordLangId, mstv.idvbmultilingualservicenamedescriptor_getrecordlangid
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
 - IDvbMultilingualServiceNameDescriptor.GetRecordLangId
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDvbMultilingualServiceNameDescriptor::GetRecordLangId


## -description


Gets the three-character ISO 639 language code from a Digital Video Broadcast (DVB) multilingual service name descriptor. The language code
identifies the language used for text in the descriptor.


## -parameters




### -param bRecordIndex [in]

Specifies the service record number,
  indexed from zero. Call the <a href="https://msdn.microsoft.com/c157e520-696f-45d8-8e43-0e6845882404">IDvbMultilingualServiceNameDescriptor::GetCountOfRecords</a>method to get the number of records in the multilingual service name descriptor.


### -param ulVal [out]

Pointer to a buffer that receives the language code. For a list of language codes, refer to <a href="http://www.sil.org/ISO639-3/codes.asp">this document</a>. 


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/1b384ecf-aa56-476d-b347-b5438ab069fe">IDvbMultilingualServiceNameDescriptor</a>



<a href="https://msdn.microsoft.com/c157e520-696f-45d8-8e43-0e6845882404">IDvbMultilingualServiceNameDescriptor::GetCountOfRecords</a>
 

 

