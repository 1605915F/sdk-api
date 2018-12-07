---
UID: NF:winddi.FLOATOBJ_MulFloat
title: FLOATOBJ_MulFloat function
author: windows-sdk-content
description: The FLOATOBJ_MulFloat function multiplies the FLOATOBJ by the value of type FLOATL, and returns with the result in the first parameter.
old-location: display\floatobj_mulfloat.htm
tech.root: display
ms.assetid: 7b4189f7-b80b-4543-b713-b0b2d06ef81e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FLOATOBJ_MulFloat, FLOATOBJ_MulFloat function [Display Devices], display.floatobj_mulfloat, gdifncs_39da7310-f7d3-4ceb-8bd5-c2a0eaab0068.xml, winddi/FLOATOBJ_MulFloat
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winddi.h
req.include-header: Winddi.h
req.target-type: Universal
req.target-min-winverclnt: Available in Windows 2000 and later versions of the Windows operating systems.
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
req.lib: Win32k.lib
req.dll: Win32k.sys
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Win32k.sys
api_name:
 - FLOATOBJ_MulFloat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FLOATOBJ_MulFloat function


## -description


The <b>FLOATOBJ_MulFloat</b> function multiplies the <a href="https://msdn.microsoft.com/5f8c401b-7487-4d75-a0a8-534fa7992a3d">FLOATOBJ</a> by the value of type FLOATL, and returns with the result in the first parameter.


## -parameters




### -param arg1 [in, out]

Pointer to the FLOATOBJ operand. When the function returns, *<i>pf</i> will be reset to the value (*<i>pf</i>  *  <i>f</i>).


### -param arg2 [in]

Specifies the FLOATL operand. This value is converted to a FLOATOBJ for the multiplication.


## -returns



None




## -remarks



The FLOATOBJ<b>_</b><i>Xxx</i> services allow graphics drivers to emulate floating-point arithmetic. An NT-based operating system does not support kernel-mode floating-point operations on some systems.




## -see-also




<a href="https://msdn.microsoft.com/5f8c401b-7487-4d75-a0a8-534fa7992a3d">FLOATOBJ</a>
 

 

