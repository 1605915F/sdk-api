---
UID: NF:sbe.IStreamBufferRecordingAttribute.SetAttribute
title: IStreamBufferRecordingAttribute::SetAttribute
author: windows-sdk-content
description: The SetAttribute method sets an attribute on the stream buffer file.
old-location: mstv\istreambufferrecordingattribute_setattribute.htm
tech.root: mstv
ms.assetid: cc441a00-e98f-4ea7-b902-d74846fc93cc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IStreamBufferRecordingAttribute interface [Microsoft TV Technologies],SetAttribute method, IStreamBufferRecordingAttribute.SetAttribute, IStreamBufferRecordingAttribute::SetAttribute, IStreamBufferRecordingAttributeSetAttribute, SetAttribute, SetAttribute method [Microsoft TV Technologies], SetAttribute method [Microsoft TV Technologies],IStreamBufferRecordingAttribute interface, mstv.istreambufferrecordingattribute_setattribute, sbe/IStreamBufferRecordingAttribute::SetAttribute
ms.topic: method
req.header: sbe.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
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
 - Sbe.h
api_name:
 - IStreamBufferRecordingAttribute.SetAttribute
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IStreamBufferRecordingAttribute::SetAttribute


## -description


The <b>SetAttribute</b> method sets an attribute on the stream buffer file.


## -parameters




### -param ulReserved [in]

Reserved. Set this parameter to zero.


### -param pszAttributeName [in]

Wide-character string that contains the name of the attribute.


### -param StreamBufferAttributeType [in]

Member of the <a href="https://msdn.microsoft.com/be478769-d9ac-4e42-b5f6-94b5656e2596">STREAMBUFFER_ATTR_DATATYPE</a> enumeration that defines the data type of the attribute data.


### -param pbAttribute [in]

Pointer to a buffer that contains the attribute data.


### -param cbAttributeLength [in]

The size of the buffer specified in <i>pbAttribute</i>.


## -returns



Returns an <b>HRESULT</b> value.




## -remarks



If an attribute with that name already exists, the method overwrites it with the new value.

The method fails if the recorder object is already recording.




## -see-also




<a href="https://msdn.microsoft.com/e72ec34e-d3e3-4f5f-9336-d55135dc1e47">IStreamBufferRecordControl::Start</a>



<a href="https://msdn.microsoft.com/7c46413f-3e51-4d72-b7f7-a8239c61b161">IStreamBufferRecordingAttribute Interface</a>
 

 

