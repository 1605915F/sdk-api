---
UID: NF:certenroll.IX509EnrollmentStatus.get_Selected
title: IX509EnrollmentStatus::get_Selected
author: windows-sdk-content
description: Specifies or retrieves a value that indicates whether an item can be used during the enrollment process.
old-location: security\ix509enrollmentstatus_selected_property.htm
tech.root: seccertenroll
ms.assetid: 9050f394-ccad-4a6e-90bc-53af3a874f91
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IX509EnrollmentStatus interface [Security],Selected property, IX509EnrollmentStatus.Selected, IX509EnrollmentStatus.get_Selected, IX509EnrollmentStatus::Selected, IX509EnrollmentStatus::get_Selected, IX509EnrollmentStatus::put_Selected, Selected property [Security], Selected property [Security],IX509EnrollmentStatus interface, certenroll/IX509EnrollmentStatus::Selected, certenroll/IX509EnrollmentStatus::get_Selected, certenroll/IX509EnrollmentStatus::put_Selected, get_Selected, security.ix509enrollmentstatus_selected_property
ms.topic: method
req.header: certenroll.h
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
req.lib: 
req.dll: CertEnroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CertEnroll.dll
api_name:
 - IX509EnrollmentStatus.Selected
 - IX509EnrollmentStatus.get_Selected
 - IX509EnrollmentStatus.put_Selected
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509EnrollmentStatus::get_Selected


## -description


The <b>Selected</b> property specifies or retrieves a value that indicates whether an item can be used during the enrollment process.

This property is read/write.


## -parameters


## -remarks



This property is currently used only to identify which cryptographic provider/algorithm pairs can be used to create a key. For more information, see the <a href="https://msdn.microsoft.com/50dc8cc5-21ee-4347-a12a-0d6e62901fbb">GetCspStatuses</a> method on the <a href="https://msdn.microsoft.com/5b3764dc-fc63-45cc-8c35-65539c461e81">IX509CertificateRequestPkcs10</a> interface.




## -see-also




<a href="https://msdn.microsoft.com/fa5e3a10-7f00-46b6-b740-b72d78745bf7">IX509EnrollmentStatus</a>
 

 

