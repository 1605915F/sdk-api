---
UID: NF:control.IBasicVideo.SetDestinationPosition
title: IBasicVideo::SetDestinationPosition
author: windows-sdk-content
description: The SetDestinationPosition method sets the destination rectangle.
old-location: dshow\ibasicvideo_setdestinationposition.htm
tech.root: DirectShow
ms.assetid: e638eb33-5a7f-4ebc-910f-72566e251f17
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IBasicVideo interface [DirectShow],SetDestinationPosition method, IBasicVideo.SetDestinationPosition, IBasicVideo::SetDestinationPosition, IBasicVideoSetDestinationPosition, SetDestinationPosition, SetDestinationPosition method [DirectShow], SetDestinationPosition method [DirectShow],IBasicVideo interface, control/IBasicVideo::SetDestinationPosition, dshow.ibasicvideo_setdestinationposition
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: control.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IBasicVideo.SetDestinationPosition
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IBasicVideo::SetDestinationPosition


## -description



The <code>SetDestinationPosition</code> method sets the destination rectangle.




## -parameters




### -param Left [in]

Specifies the x-coordinate, in pixels.


### -param Top [in]

Specifies the y-coordinate, in pixels.


### -param Width [in]

Specifies the width, in pixels.


### -param Height [in]

Specifies the height, in pixels.


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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument. <i>Width</i> and <i>Height</i> must be larger than zero.

</td>
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
<tr>
<td width="40%">
<dl>
<dt><b>VFW_E_NOT_CONNECTED</b></dt>
</dl>
</td>
<td width="60%">
The video renderer is not connected.

</td>
</tr>
</table>
 




## -remarks



This method has the same effect as individually calling the <a href="https://msdn.microsoft.com/en-us/library/Dd389591(v=VS.85).aspx">IBasicVideo::put_DestinationLeft</a>, <a href="https://msdn.microsoft.com/en-us/library/Dd389592(v=VS.85).aspx">IBasicVideo::put_DestinationTop</a>, <a href="https://msdn.microsoft.com/en-us/library/Dd389593(v=VS.85).aspx">IBasicVideo::put_DestinationWidth</a>, and <a href="https://msdn.microsoft.com/en-us/library/Dd389590(v=VS.85).aspx">IBasicVideo::put_DestinationHeight</a> methods.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd375623(v=VS.85).aspx">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd389540(v=VS.85).aspx">IBasicVideo Interface</a>
 

 

