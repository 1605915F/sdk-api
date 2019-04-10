---
UID: NS:ddrawint._DD_GETBLTSTATUSDATA
title: DD_GETBLTSTATUSDATA (ddrawint.h)
author: windows-sdk-content
description: The DD_GETBLTSTATUSDATA structure returns the blit status information.
old-location: display\dd_getbltstatusdata.htm
tech.root: display
ms.assetid: 16b0cac9-af8c-4106-b74e-6c9ada543851
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDD_GETBLTSTATUSDATA, DD_GETBLTSTATUSDATA, DD_GETBLTSTATUSDATA structure [Display Devices], ddrawint/DD_GETBLTSTATUSDATA, ddstrcts_fec10d7e-ffc0-4368-8cd8-e1028ac7874d.xml, display.dd_getbltstatusdata"
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
 - DD_GETBLTSTATUSDATA
product: Windows
targetos: Windows
req.typenames: "*PDD_GETBLTSTATUSDATA, DD_GETBLTSTATUSDATA"
req.redist: 
---

# DD_GETBLTSTATUSDATA structure


## -description


The DD_GETBLTSTATUSDATA structure returns the blit status information.


## -struct-fields




### -field lpDD

Points to a <a href="https://msdn.microsoft.com/a59f064b-48cf-4491-82cd-84f59467af87">DD_DIRECTDRAW_GLOBAL</a> structure that describes the driver's device.


### -field lpDDSurface

Points to a <a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a> structure representing the surface whose blit status is being queried. 


### -field dwFlags

Specifies the blit status being requested. This member can be one of the following values:

<table>
<tr>
<th>Flag</th>
<th>Meaning</th>
</tr>
<tr>
<td>
DDGBS_CANBLT

</td>
<td>
Queries whether the driver can currently perform a blit.

</td>
</tr>
<tr>
<td>
DDGBS_ISBLTDONE

</td>
<td>
Queries whether the driver has completed the last blit.

</td>
</tr>
</table>
 


### -field ddRVal

Specifies the location in which the driver writes the return value of the <a href="https://msdn.microsoft.com/77cce7a4-a0e6-48f7-933f-a216b13ddc93">DdGetBltStatus</a> callback. A return code of DD_OK indicates success. For more information, see <a href="https://msdn.microsoft.com/da4cc7d7-6826-48aa-96c6-004e31fc3e3e">Return Values for DirectDraw</a>.


### -field GetBltStatus

Used by the Microsoft DirectDraw API and should not be filled in by the driver.


## -see-also




<a href="https://msdn.microsoft.com/77cce7a4-a0e6-48f7-933f-a216b13ddc93">DdGetBltStatus</a>
 

 

