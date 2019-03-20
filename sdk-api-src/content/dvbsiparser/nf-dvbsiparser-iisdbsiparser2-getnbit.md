---
UID: NF:dvbsiparser.IIsdbSiParser2.GetNBIT
title: IIsdbSiParser2::GetNBIT (dvbsiparser.h)
author: windows-sdk-content
description: Gets the network board information table (NBIT) from an Integrated Services Digital Broadcast (ISDB) transport stream. The NBIT describes the programs included in a multiplexed transport stream.
old-location: mstv\iisdbsiparser2_getnbit.htm
tech.root: mstv
ms.assetid: 90c47d88-b364-4b42-b51b-dfa3c9eed4b0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetNBIT, GetNBIT method [Microsoft TV Technologies], GetNBIT method [Microsoft TV Technologies],IIsdbSiParser2 interface, IIsdbSiParser2 interface [Microsoft TV Technologies],GetNBIT method, IIsdbSiParser2.GetNBIT, IIsdbSiParser2::GetNBIT, dvbsiparser/IIsdbSiParser2::GetNBIT, mstv.iisdbsiparser2_getnbit
ms.topic: method
req.header: dvbsiparser.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - IIsdbSiParser2.GetNBIT
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IIsdbSiParser2::GetNBIT


## -description


Gets the network board information table (NBIT) from an Integrated Services Digital Broadcast (ISDB) transport stream.
  The NBIT describes the programs included in a multiplexed transport stream.



## -parameters




### -param tableId [in]

Table identifier for the type of table to retrieve. For an NBIT, this value is 0xC5 if the table contains the network board information body, or 0xC6 if the table contains reference information for retrieving the network board information.


### -param pwOriginalNetworkId

Pointer to the original_network_id field for the NBIT. This field contains an identifier for the broadcaster that originates the
  MPEG-2 transport stream


### -param ppNBIT [out]

Receives a pointer to the <a href="https://msdn.microsoft.com/32c15a03-6683-4b22-b374-a15784696368">IISDB_NBIT</a>interface. Use this interface to retrieve the information in the table. 
The caller must release the interface.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/32c15a03-6683-4b22-b374-a15784696368">IISDB_NBIT</a>



<a href="https://msdn.microsoft.com/d8dfc713-aaa4-46b1-8eca-2e132a9d705f">IIsdbSiParser2</a>
 

 

