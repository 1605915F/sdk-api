---
UID: NF:dvbsiparser.IPBDAAttributesDescriptor.GetAttributePayload
title: IPBDAAttributesDescriptor::GetAttributePayload
author: windows-sdk-content
description: Gets the descriptor body from an attributes descriptor in a Protected Broadcast Device Architecture (PBDA) transport stream.
old-location: mstv\ipbdaattributesdescriptor_getattributepayload.htm
tech.root: mstv
ms.assetid: 315f6afe-a5cc-4fe2-8029-fcf280b358b2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAttributePayload, GetAttributePayload method [Microsoft TV Technologies], GetAttributePayload method [Microsoft TV Technologies],IPBDAAttributesDescriptor interface, IPBDAAttributesDescriptor interface [Microsoft TV Technologies],GetAttributePayload method, IPBDAAttributesDescriptor.GetAttributePayload, IPBDAAttributesDescriptor::GetAttributePayload, dvbsiparser/IPBDAAttributesDescriptor::GetAttributePayload, mstv.ipbdaattributesdescriptor_getattributepayload
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
 - IPBDAAttributesDescriptor.GetAttributePayload
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPBDAAttributesDescriptor::GetAttributePayload


## -description


Gets the descriptor body from an attributes descriptor in a Protected Broadcast  Device Architecture (PBDA) transport stream.


## -parameters




### -param ppbAttributeBuffer [out]

Pointer to a buffer that receives the descriptor body. The caller must free this memory after use.


### -param pdwAttributeLength [out]

Receives the descriptor body length.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/489348b7-0f10-4a49-a7d4-10a1ed478aa8">IPBDAAttributesDescriptor</a>
 

 

