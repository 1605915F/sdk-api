---
UID: NS:wmsdkidl._WMT_FILESINK_DATA_UNIT
title: WMT_FILESINK_DATA_UNIT
author: windows-sdk-content
description: The WMT_FILESINK_DATA_UNIT structure is used by IWMWriterFileSink3::OnDataUnitEx to deliver information about a packet.
old-location: wmformat\wmt_filesink_data_unit.htm
tech.root: wmformat
ms.assetid: e1deb01f-9f53-4ede-a3e1-13d6dc79adb5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WMT_FILESINK_DATA_UNIT, WMT_FILESINK_DATA_UNIT structure [windows Media Format], wmformat.wmt_filesink_data_unit, wmsdkidl/WMT_FILESINK_DATA_UNIT
ms.topic: struct
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - HeaderDef
api_location:
 - Wmsdkidl.h
api_name:
 - WMT_FILESINK_DATA_UNIT
product: Windows
targetos: Windows
req.typenames: WMT_FILESINK_DATA_UNIT
req.redist: 
---

# WMT_FILESINK_DATA_UNIT structure


## -description



The <b>WMT_FILESINK_DATA_UNIT</b> structure is used by <b>IWMWriterFileSink3::OnDataUnitEx</b> to deliver information about a packet.




## -struct-fields




### -field packetHeaderBuffer

A <a href="https://msdn.microsoft.com/047e19da-c819-46e5-8a1c-09bc93a05259">WMT_BUFFER_SEGMENT</a> structure specifying the buffer segment that contains the packet header.


### -field cPayloads

Count of payloads in this packet. This is also the number of elements in the array specified in <b>pPayloadHeaderBuffers</b>.


### -field pPayloadHeaderBuffers

Pointer to an array of <b>WMT_BUFFER_SEGMENT</b> structures. Each element specifies a buffer segment that contains a payload header. The number of elements is specified by <b>cPayloads</b>.


### -field cPayloadDataFragments

Count of payload data fragments in this packet. This is also the number of elements in the array pointed to by <b>pPayloadDataFragments</b>.


### -field pPayloadDataFragments

Pointer to an array of <a href="https://msdn.microsoft.com/5a99c772-0e8a-4f6d-a13f-9bf7b4fa7d89">WMT_PAYLOAD_FRAGMENT</a> structures. Each element specifies a buffer segment that contains a payload fragment. The number of elements is specified by <b>cPayloadDataFragments</b>.


## -see-also




<a href="https://msdn.microsoft.com/1dbcb27b-7588-4475-99fe-3e547d1659d3">IWMWriterFileSink3::OnDataUnitEx</a>



<a href="https://msdn.microsoft.com/118ef278-ca4f-4c30-9633-a2d851f5c758">Structures</a>
 

 

