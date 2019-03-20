---
UID: NS:lmalert._ADMIN_OTHER_INFO
title: ADMIN_OTHER_INFO (lmalert.h)
author: windows-sdk-content
description: The ADMIN_OTHER_INFO structure contains error message information. The NetAlertRaise and NetAlertRaiseEx functions use the ADMIN_OTHER_INFO structure to specify information when raising an administrator's interrupting message.
old-location: netmgmt\admin_other_info_str.htm
tech.root: NetMgmt
ms.assetid: 43119dcf-7d04-4e3b-b1dc-20e814fbdc2f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPADMIN_OTHER_INFO, *PADMIN_OTHER_INFO, ADMIN_OTHER_INFO, ADMIN_OTHER_INFO structure [Network Management], LPADMIN_OTHER_INFO, LPADMIN_OTHER_INFO structure pointer [Network Management], PADMIN_OTHER_INFO, PADMIN_OTHER_INFO structure pointer [Network Management], _win32_admin_other_info_str, lmalert/ADMIN_OTHER_INFO, lmalert/LPADMIN_OTHER_INFO, lmalert/PADMIN_OTHER_INFO, netmgmt.admin_other_info_str"
ms.topic: struct
req.header: lmalert.h
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
 - Lmalert.h
api_name:
 - ADMIN_OTHER_INFO
product: Windows
targetos: Windows
req.typenames: ADMIN_OTHER_INFO, *PADMIN_OTHER_INFO, *LPADMIN_OTHER_INFO
req.redist: 
---

# ADMIN_OTHER_INFO structure


## -description


The
				<b>ADMIN_OTHER_INFO</b> structure contains error message information. The 
<a href="https://msdn.microsoft.com/11367a72-c21d-4044-98cf-a7a30cc43a8b">NetAlertRaise</a> and 
<a href="https://msdn.microsoft.com/9762f0d6-0022-4e05-b2d8-6223d7bbb2c8">NetAlertRaiseEx</a> functions use the 
<b>ADMIN_OTHER_INFO</b> structure to specify information when raising an administrator's interrupting message.


## -struct-fields




### -field alrtad_errcode

Specifies the error code for the new message written to the message log.


### -field alrtad_numstrings

Specifies the number (0-9) of consecutive Unicode strings written to the message log.


## -remarks



Variable-length data follows the 
<b>ADMIN_OTHER_INFO</b> structure in the alert message buffer if you specify one or more strings in the <b>alrtad_numstrings</b> member. The calling application must allocate and free the memory for all structures and variable-length data in an alert message buffer.

See 
<a href="https://msdn.microsoft.com/11367a72-c21d-4044-98cf-a7a30cc43a8b">NetAlertRaise</a> and 
<a href="https://msdn.microsoft.com/9762f0d6-0022-4e05-b2d8-6223d7bbb2c8">NetAlertRaiseEx</a> for code samples that demonstrate how to raise an administrative alert.




## -see-also




<a href="https://msdn.microsoft.com/e131191b-7413-45ff-84cd-b3a873d33ca1">Alert Functions</a>



<a href="https://msdn.microsoft.com/832ebe88-e1c4-4ce3-8057-922419b577f7">ERRLOG_OTHER_INFO</a>



<a href="https://msdn.microsoft.com/11367a72-c21d-4044-98cf-a7a30cc43a8b">NetAlertRaise</a>



<a href="https://msdn.microsoft.com/9762f0d6-0022-4e05-b2d8-6223d7bbb2c8">NetAlertRaiseEx</a>



<a href="https://msdn.microsoft.com/426c7b2e-027c-4a88-97b7-eba5201d0f0d">Network Management Overview</a>



<a href="https://msdn.microsoft.com/a4b05054-bef2-4cab-89f6-725d92ee75b8">Network Management Structures</a>



<a href="https://msdn.microsoft.com/f2fd87bc-abde-43c0-b29d-d43cc5f038b8">PRINT_OTHER_INFO</a>



<a href="https://msdn.microsoft.com/daa4594f-e59e-4f05-8183-677bee4ea446">STD_ALERT</a>



<a href="https://msdn.microsoft.com/2f6bd906-fdab-410a-8856-4482e047371f">USER_OTHER_INFO</a>
 

 

