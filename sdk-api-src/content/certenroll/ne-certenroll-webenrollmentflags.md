---
UID: NE:certenroll.WebEnrollmentFlags
title: WebEnrollmentFlags (certenroll.h)
author: windows-sdk-content
description: Specifies web enrollment behavior.
old-location: security\webenrollmentflags.htm
tech.root: seccertenroll
ms.assetid: 3b5940c4-f262-498e-82ab-c56af13afd06
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EnrollPrompt, WebEnrollmentFlags, WebEnrollmentFlags enumeration [Security], certenroll/EnrollPrompt, certenroll/WebEnrollmentFlags, security.webenrollmentflags
ms.topic: enum
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - Certenroll.h
api_name:
 - WebEnrollmentFlags
product: Windows
targetos: Windows
req.typenames: WebEnrollmentFlags
req.redist: 
---

# WebEnrollmentFlags enumeration


## -description


The <b>WebEnrollmentFlags</b> enumeration specifies web enrollment behavior. It is used by the <a href="https://msdn.microsoft.com/4f178df7-714f-49e6-9bf5-647acc23b0ad">Enroll</a> method on the <a href="https://msdn.microsoft.com/19124591-be1a-401e-9b83-c640d00de34a">IX509EnrollmentHelper</a> interface.


## -enum-fields




### -field EnrollPrompt

If this flag is set and no authentication credential is available for the certificate enrollment server, the certificate service prompts for a credential. If there is no authentication credential and this flag is not set, the <a href="https://msdn.microsoft.com/4f178df7-714f-49e6-9bf5-647acc23b0ad">Enroll</a> method fails.


## -see-also




<a href="https://msdn.microsoft.com/4f178df7-714f-49e6-9bf5-647acc23b0ad">Enroll</a>



<a href="https://msdn.microsoft.com/19124591-be1a-401e-9b83-c640d00de34a">IX509EnrollmentHelper</a>
 

 

