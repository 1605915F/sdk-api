---
UID: NF:bdatif.IMPEG2_TIF_CONTROL.GetPIDs
title: IMPEG2_TIF_CONTROL::GetPIDs (bdatif.h)
author: windows-sdk-content
description: The GetPIDs method retrieves the list of MPEG-2 Packet IDs being filtered into the TIF's input data.
old-location: mstv\impeg2_tif_control_getpids.htm
tech.root: mstv
ms.assetid: c7ca141b-e471-47ce-96b5-b2c0cad89daf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPIDs, GetPIDs method [Microsoft TV Technologies], GetPIDs method [Microsoft TV Technologies],IMPEG2_TIF_CONTROL interface, IMPEG2_TIF_CONTROL interface [Microsoft TV Technologies],GetPIDs method, IMPEG2_TIF_CONTROL.GetPIDs, IMPEG2_TIF_CONTROL::GetPIDs, IMPEG2_TIF_CONTROLGetPIDs, bdatif/IMPEG2_TIF_CONTROL::GetPIDs, mstv.impeg2_tif_control_getpids
ms.topic: method
req.header: bdatif.h
req.include-header: 
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
 - COM
api_location:
 - bdatif.h
api_name:
 - IMPEG2_TIF_CONTROL.GetPIDs
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMPEG2_TIF_CONTROL::GetPIDs


## -description



The <b>GetPIDs</b> method retrieves the list of MPEG-2 Packet IDs being filtered into the TIF's input data.




## -parameters




### -param pulcPIDs [out]

Pointer to a variable that receives the number of PIDs that were retrieved.


### -param pulPIDs [out]

Pointer to a variable that receives an array of returned <b>ULONG</b> values representing the PID values. The number of elements in the array is equal to the value of <i>pulcPIDs</i>.


## -returns



The method returns an <b>HRESULT</b>. Possible values include those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



A custom TIF extension might or might not have need for this method.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/9583365d-b318-49e2-a32f-f6cc9d3f289d">IMPEG2_TIF_CONTROL Interface</a>



<a href="https://msdn.microsoft.com/27add7cc-1d77-4ac5-b63f-757f63f4c9b8">IMPEG2_TIF_CONTROL::AddPIDs</a>



<a href="https://msdn.microsoft.com/2d77c3d8-b91c-43de-b4c1-bd41636eb4ad">IMPEG2_TIF_CONTROL::GetPIDCount</a>
 

 

