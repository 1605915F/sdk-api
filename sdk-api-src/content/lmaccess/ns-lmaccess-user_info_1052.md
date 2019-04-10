---
UID: NS:lmaccess._USER_INFO_1052
title: USER_INFO_1052 (lmaccess.h)
author: windows-sdk-content
description: The USER_INFO_1052 structure contains the path to a network user's profile. This information level is valid only when you call the NetUserSetInfo function.
old-location: netmgmt\user_info_1052_str.htm
tech.root: NetMgmt
ms.assetid: 55ec6819-8558-413a-9a79-c2d59993163d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPUSER_INFO_1052, *PUSER_INFO_1052, LPUSER_INFO_1052, LPUSER_INFO_1052 structure pointer [Network Management], PUSER_INFO_1052, PUSER_INFO_1052 structure pointer [Network Management], USER_INFO_1052, USER_INFO_1052 structure [Network Management], _win32_user_info_1052_str, lmaccess/LPUSER_INFO_1052, lmaccess/PUSER_INFO_1052, lmaccess/USER_INFO_1052, netmgmt.user_info_1052_str"
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
 - USER_INFO_1052
product: Windows
targetos: Windows
req.typenames: USER_INFO_1052, *PUSER_INFO_1052, *LPUSER_INFO_1052
req.redist: 
---

# USER_INFO_1052 structure


## -description


The
				<b>USER_INFO_1052</b> structure contains the path to a network user's profile. This information level is valid only when you call the 
<a href="https://msdn.microsoft.com/ffe49d4b-e7e8-4982-8087-59bb7534b257">NetUserSetInfo</a> function.


## -struct-fields




### -field usri1052_profile

Specifies a Unicode string that contains the path to the user's profile. The user is specified in the <i>username</i> parameter to the 
<b>NetUserSetInfo</b> function. This value can be a null string, a local absolute path, or a UNC path.


## -see-also




<a href="https://msdn.microsoft.com/ffe49d4b-e7e8-4982-8087-59bb7534b257">NetUserSetInfo</a>



<a href="https://msdn.microsoft.com/426c7b2e-027c-4a88-97b7-eba5201d0f0d">Network Management Overview</a>



<a href="https://msdn.microsoft.com/a4b05054-bef2-4cab-89f6-725d92ee75b8">Network Management Structures</a>



<a href="https://msdn.microsoft.com/cf0e5102-3924-46c0-8124-0aa04e95f48d">User Functions</a>
 

 

