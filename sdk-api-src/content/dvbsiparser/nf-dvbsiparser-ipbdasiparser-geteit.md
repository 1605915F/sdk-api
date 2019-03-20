---
UID: NF:dvbsiparser.IPBDASiParser.GetEIT
title: IPBDASiParser::GetEIT (dvbsiparser.h)
author: windows-sdk-content
description: Gets the event information table (EIT) from the program and system information protocol (PSIP) tables in a Protected Broadcast Device Architecture (PBDA) transport stream.
old-location: mstv\ipbdasiparser_geteit.htm
tech.root: mstv
ms.assetid: ab7df40a-6a1c-4017-bece-618fb75797cf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetEIT, GetEIT method [Microsoft TV Technologies], GetEIT method [Microsoft TV Technologies],IPBDASiParser interface, IPBDASiParser interface [Microsoft TV Technologies],GetEIT method, IPBDASiParser.GetEIT, IPBDASiParser::GetEIT, dshow.ipbdasiparser_geteit, dvbsiparser/IPBDASiParser::GetEIT, mstv.ipbdasiparser_geteit
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
 - IPBDASiParser.GetEIT
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPBDASiParser::GetEIT


## -description


Gets the event information table (EIT) from  the program and system information protocol (PSIP) tables in a Protected Broadcast  Device Architecture (PBDA) transport stream.


## -parameters




### -param dwSize [in]

Reserved. Set to zero.


### -param pBuffer [in]

Reserved. Set to <b>NULL</b>.


### -param ppEIT [out]

Receives a pointer to the <a href="https://msdn.microsoft.com/cb8cd2cc-e498-43c2-ae1e-3543b4ea3b56">IPBDA_EIT</a> interface.  The caller must release the interface.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/a1cc25ec-b519-4c24-ba85-f2c240749fbd">IPBDASiParser</a>
 

 

