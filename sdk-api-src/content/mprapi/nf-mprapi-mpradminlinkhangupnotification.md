---
UID: NF:mprapi.MprAdminLinkHangupNotification
title: MprAdminLinkHangupNotification function (mprapi.h)
author: windows-sdk-content
description: RAS calls the MprAdminLinkHangupNotification function whenever a link for a particular connection is dismantled.
old-location: rras\mpradminlinkhangupnotification.htm
tech.root: RRAS
ms.assetid: 7f2b30e8-ba1d-4db3-843f-f9eafca47add
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MprAdminLinkHangupNotification, MprAdminLinkHangupNotification callback, MprAdminLinkHangupNotification callback function [RAS], _mpr_mpradminlinkhangupnotification, mprapi/MprAdminLinkHangupNotification, rras.mpradminlinkhangupnotification
ms.topic: function
req.header: mprapi.h
req.include-header: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Mprapi.h
api_name:
 - MprAdminLinkHangupNotification
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MprAdminLinkHangupNotification function


## -description


RAS calls the 
<b>MprAdminLinkHangupNotification</b> function whenever a link for a particular connection is dismantled.


## -parameters




### -param pRasPort0 [in]

Pointer to a 
<a href="https://msdn.microsoft.com/361b065e-8240-465f-a0fe-d4bfc097ec70">RAS_PORT_0</a> structure that describes the port being used by the link.


### -param pRasPort1 [in]

Pointer to a 
<a href="https://msdn.microsoft.com/4850f08e-13ee-485f-99a5-be4554d6311b">RAS_PORT_1</a> structure that describes the port being used by the link.


## -returns



This function does not have a return value.




## -remarks



RAS supports multiple Administration DLLs. RAS calls the multiple implementations of 
<b>MprAdminLinkHangupNotification</b> in the order in which the DLLs are listed in the 
<a href="https://msdn.microsoft.com/e83a5e37-a39d-4465-abc9-653cdd56893b">registry</a>.

<b>Windows 2000 Server and earlier:  </b>If RAS does not accept the new link, RAS does not call the 
<b>MprAdminLinkHangupNotification</b> function.

Do not call any of the 
<a href="https://msdn.microsoft.com/27cf63e2-9dd3-4bc1-98af-e93055d89492">RAS Administration Functions</a> or 
<a href="https://msdn.microsoft.com/e58fa4a6-16d3-4953-bf21-887d08e25af7">RAS User Administration Functions</a> from inside 
<b>MprAdminLinkHangupNotification</b>. Calls to these functions will not return when made from within a callout function.




## -see-also




<a href="https://msdn.microsoft.com/6ca7fe28-53e1-49e0-ab3c-4e8e4343c88c">MprAdminAcceptNewConnection</a>



<a href="https://msdn.microsoft.com/72cdcb3c-c44c-405c-ab4b-93bf9c628acf">MprAdminAcceptNewConnection2</a>



<a href="https://msdn.microsoft.com/a4cbca7d-a8b0-4396-9201-648bcca6a8c8">MprAdminAcceptNewLink</a>



<a href="https://msdn.microsoft.com/504ce881-7d06-41d3-a942-0fe27be12bd3">MprAdminConnectionHangupNotification</a>



<a href="https://msdn.microsoft.com/3231ae83-c7fc-46d4-a4d9-f7ccf1c4ed18">MprAdminConnectionHangupNotification2</a>



<a href="https://msdn.microsoft.com/c15c6e2d-3bb6-4583-9ac3-19528feb863f">RAS Administration DLL</a>



<a href="https://msdn.microsoft.com/27cf63e2-9dd3-4bc1-98af-e93055d89492">RAS Administration Functions</a>



<a href="https://msdn.microsoft.com/361b065e-8240-465f-a0fe-d4bfc097ec70">RAS_PORT_0</a>



<a href="https://msdn.microsoft.com/4850f08e-13ee-485f-99a5-be4554d6311b">RAS_PORT_1</a>



<a href="https://msdn.microsoft.com/6170fcf2-26d5-4418-bddb-2afd99510520">Remote Access Service Administration Reference</a>
 

 

