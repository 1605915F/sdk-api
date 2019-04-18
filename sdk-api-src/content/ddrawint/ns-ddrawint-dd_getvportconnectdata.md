---
UID: NS:ddrawint._DD_GETVPORTCONNECTDATA
title: DD_GETVPORTCONNECTDATA (ddrawint.h)
author: windows-sdk-content
description: The DD_GETVPORTCONNECTDATA structure contains the connection combinations supported by the specified video port extensions (VPE) object.
old-location: display\dd_getvportconnectdata.htm
tech.root: display
ms.assetid: 74cea50f-b8fd-4c32-815f-19f075b74838
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDD_GETVPORTCONNECTDATA, DD_GETVPORTCONNECTDATA, DD_GETVPORTCONNECTDATA structure [Display Devices], ddrawint/DD_GETVPORTCONNECTDATA, ddstrcts_56b2c83f-8798-4960-8fb6-062ccd1d5dd3.xml, display.dd_getvportconnectdata"
ms.topic: struct
req.header: ddrawint.h
req.include-header: Winddi.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - ddrawint.h
api_name:
 - DD_GETVPORTCONNECTDATA
product: Windows
targetos: Windows
req.typenames: "*PDD_GETVPORTCONNECTDATA, DD_GETVPORTCONNECTDATA"
req.redist: 
ms.custom: 19H1
---

# DD_GETVPORTCONNECTDATA structure


## -description


The DD_GETVPORTCONNECTDATA structure contains the connection combinations supported by the specified <a href="https://msdn.microsoft.com/a1de1905-09f3-4689-ace9-06690a1f930a">video port extensions (VPE)</a> object.


## -struct-fields




### -field lpDD

Points to a <a href="https://msdn.microsoft.com/58e378b7-863a-46d4-91cb-904ed4e892a3">DD_DIRECTDRAW_LOCAL</a> structure that is relevant to the current Microsoft DirectDraw process only.


### -field dwPortId

Specifies the ID of the VPE object for which the driver is to retrieve connection information. DirectDraw obtains this ID from the <b>dwVideoPortID</b> member of the <a href="https://msdn.microsoft.com/ea85f189-7308-48ad-b159-1809749f8183">DDVIDEOPORTCAPS</a> structure.


### -field lpConnect

Points to an array of <a href="https://msdn.microsoft.com/54c1bb05-37a8-4841-808b-2eb9d1ecd7a3">DDVIDEOPORTCONNECT</a> structures in which the driver should return the characteristics of each connection that the VPE object supports. This member can be <b>NULL</b>.


### -field dwNumEntries

Specifies the location in which the driver returns the number of connection combinations supported by the specified VPE object.


### -field ddRVal

Specifies the location in which the driver writes the return value of the <a href="https://msdn.microsoft.com/b6be5f94-6d4d-4f7a-a8d9-15bfc7a15d3b">DdVideoPortGetConnectInfo</a> callback. A return code of DD_OK indicates success. For more information, see <a href="https://msdn.microsoft.com/da4cc7d7-6826-48aa-96c6-004e31fc3e3e">Return Values for DirectDraw</a>.


### -field GetVideoPortConnectInfo

Used by the DirectDraw API and should not be filled in by the driver.


## -see-also




<a href="https://msdn.microsoft.com/ea85f189-7308-48ad-b159-1809749f8183">DDVIDEOPORTCAPS</a>



<a href="https://msdn.microsoft.com/54c1bb05-37a8-4841-808b-2eb9d1ecd7a3">DDVIDEOPORTCONNECT</a>



<a href="https://msdn.microsoft.com/b6be5f94-6d4d-4f7a-a8d9-15bfc7a15d3b">DdVideoPortGetConnectInfo</a>
 

 

