---
UID: NS:lmaccess._USER_INFO_1011
title: USER_INFO_1011 (lmaccess.h)
author: windows-sdk-content
description: The USER_INFO_1011 structure contains the full name of a network user. This information level is valid only when you call the NetUserSetInfo function.
old-location: netmgmt\user_info_1011_str.htm
tech.root: NetMgmt
ms.assetid: f60075b4-19c5-4998-b8c3-61e960e76035
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPUSER_INFO_1011, *PUSER_INFO_1011, LPUSER_INFO_1011, LPUSER_INFO_1011 structure pointer [Network Management], PUSER_INFO_1011, PUSER_INFO_1011 structure pointer [Network Management], USER_INFO_1011, USER_INFO_1011 structure [Network Management], _win32_user_info_1011_str, lmaccess/LPUSER_INFO_1011, lmaccess/PUSER_INFO_1011, lmaccess/USER_INFO_1011, netmgmt.user_info_1011_str"
ms.topic: struct
req.header: lmaccess.h
req.include-header: Lm.h
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
 - HeaderDef
api_location:
 - Lmaccess.h
api_name:
 - USER_INFO_1011
product: Windows
targetos: Windows
req.typenames: USER_INFO_1011, *PUSER_INFO_1011, *LPUSER_INFO_1011
req.redist: 
ms.custom: 19H1
---

# USER_INFO_1011 structure


## -description


The
				<b>USER_INFO_1011</b> structure contains the full name of a network user. This information level is valid only when you call the 
<a href="https://msdn.microsoft.com/ffe49d4b-e7e8-4982-8087-59bb7534b257">NetUserSetInfo</a> function.


## -struct-fields




### -field usri1011_full_name

Pointer to a Unicode string that contains the full name of the user. The user is specified in the <i>username</i> parameter to the 
<b>NetUserSetInfo</b> function. This string can be a null string, or it can have any number of characters before the terminating null character.


## -see-also




<a href="https://msdn.microsoft.com/ffe49d4b-e7e8-4982-8087-59bb7534b257">NetUserSetInfo</a>



<a href="https://msdn.microsoft.com/426c7b2e-027c-4a88-97b7-eba5201d0f0d">Network Management Overview</a>



<a href="https://msdn.microsoft.com/a4b05054-bef2-4cab-89f6-725d92ee75b8">Network Management Structures</a>



<a href="https://msdn.microsoft.com/cf0e5102-3924-46c0-8124-0aa04e95f48d">User Functions</a>
 

 

