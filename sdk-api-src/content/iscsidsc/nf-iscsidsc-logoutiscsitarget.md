---
UID: NF:iscsidsc.LogoutIScsiTarget
title: LogoutIScsiTarget function (iscsidsc.h)
author: windows-sdk-content
description: The LogoutIscsiTarget routine closes the specified login session.
old-location: iscsidisc\logoutiscsitarget.htm
tech.root: iSCSIDisc
ms.assetid: c49ad2e2-3f06-48e7-bf38-6074f9a6bcad
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: LogoutIScsiTarget, LogoutIscsiTarget, LogoutIscsiTarget function [iSCSI Discovery Library API], iscsidisc.logoutiscsitarget, iscsidsc/LogoutIscsiTarget
ms.topic: function
req.header: iscsidsc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Iscsidsc.lib
req.dll: Iscsidsc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Iscsidsc.dll
api_name:
 - LogoutIscsiTarget
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# LogoutIScsiTarget function


## -description


The <b>LogoutIscsiTarget</b> routine closes the specified login session.


## -parameters




### -param UniqueSessionId [in]

A pointer to a structure of type <a href="https://msdn.microsoft.com/d13975f9-58d0-425c-a2de-a0d1d70850d3">ISCSI_UNIQUE_SESSION_ID</a> that contains a unique session identifier for the login session end.


## -returns



Returns ERROR_SUCCESS if the operation succeeds. Otherwise, it returns the appropriate Win32 or iSCSI error code.





## -remarks



If the login session is not for informational purposes, the iSCSI initiator service ensures that all devices associated with the session can be safely removed from the device stack before allowing the initiator to close the session. If the session is an informational session, the iSCSI initiator service closes the session immediately.






## -see-also




<a href="https://msdn.microsoft.com/d13975f9-58d0-425c-a2de-a0d1d70850d3">ISCSI_UNIQUE_SESSION_ID</a>



<a href="https://msdn.microsoft.com/e94e72d2-b93c-41f4-aafc-78e6a97d7a26">LoginIscsiTarget</a>
 

 

