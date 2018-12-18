---
UID: NF:msvidctl.IMSVidCtl.get_MaintainAspectRatio
title: IMSVidCtl::get_MaintainAspectRatio
author: windows-sdk-content
description: The get_MaintainAspectRatio method queries whether the Video Control maintains the aspect ratio of the source video.
old-location: mstv\imsvidctl_get_maintainaspectratio.htm
tech.root: mstv
ms.assetid: eebb75d2-d5ee-49d6-b1bf-03b0040564b7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidCtl interface [Microsoft TV Technologies],get_MaintainAspectRatio method, IMSVidCtl.get_MaintainAspectRatio, IMSVidCtl::get_MaintainAspectRatio, IMSVidCtlget_MaintainAspectRatio, get_MaintainAspectRatio, get_MaintainAspectRatio method [Microsoft TV Technologies], get_MaintainAspectRatio method [Microsoft TV Technologies],IMSVidCtl interface, mstv.imsvidctl_get_maintainaspectratio, msvidctl/IMSVidCtl::get_MaintainAspectRatio
ms.topic: method
req.header: msvidctl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Msvidctl.idl
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
 - msvidctl.h
api_name:
 - IMSVidCtl.get_MaintainAspectRatio
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidCtl::get_MaintainAspectRatio


## -description


The <b>get_MaintainAspectRatio</b> method queries whether the Video Control maintains the aspect ratio of the source video.


## -parameters




### -param CurrentValue [out]

Receives one of the following values.

<table>
<tr>
<th>Value
                </th>
<th>Description
                </th>
</tr>
<tr>
<td>VARIANT_TRUE</td>
<td>The Video Control will maintain the aspect ratio of the source video.</td>
</tr>
<tr>
<td>VARIANT_FALSE</td>
<td>The Video Control will stretch the video to fill the window.</td>
</tr>
</table>
 


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

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
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
NULL pointer argument.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/e3ea10ea-bfb4-4c35-9933-5ad0367fd9ee">IMSVidCtl Interface</a>



<a href="https://msdn.microsoft.com/7f0943b1-3cb9-46dc-8aaf-be22e2464092">IMSVidCtl::put_MaintainAspectRatio</a>
 

 

