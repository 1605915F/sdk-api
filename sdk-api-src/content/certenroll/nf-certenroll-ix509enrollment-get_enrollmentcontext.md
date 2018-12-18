---
UID: NF:certenroll.IX509Enrollment.get_EnrollmentContext
title: IX509Enrollment::get_EnrollmentContext
author: windows-sdk-content
description: Retrieves an enrollment context that identifies whether the certificate is intended for a computer or an end-user.
old-location: security\ix509enrollment_enrollmentcontext_property.htm
tech.root: seccertenroll
ms.assetid: 48bfe2cd-1d17-42a9-8068-b635fd220911
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnrollmentContext property [Security], EnrollmentContext property [Security],IX509Enrollment interface, IX509Enrollment interface [Security],EnrollmentContext property, IX509Enrollment.EnrollmentContext, IX509Enrollment.get_EnrollmentContext, IX509Enrollment::EnrollmentContext, IX509Enrollment::get_EnrollmentContext, certenroll/IX509Enrollment::EnrollmentContext, certenroll/IX509Enrollment::get_EnrollmentContext, get_EnrollmentContext, security.ix509enrollment_enrollmentcontext_property
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
 - IX509Enrollment.EnrollmentContext
 - IX509Enrollment.get_EnrollmentContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509Enrollment::get_EnrollmentContext


## -description


The <b>EnrollmentContext</b> property retrieves an enrollment context that identifies whether the certificate is intended for a computer or an end-user.

This property is read-only.


## -parameters


## -remarks



Before calling this property, you must initialize the <a href="https://msdn.microsoft.com/37f1dd3b-bbe9-40ab-87c9-2405d97f5541">IX509Enrollment</a> object by calling one of the following methods.<ul>
<li>
<a href="https://msdn.microsoft.com/3bf4ce4a-6556-403c-8334-a6bf01f074a3">Initialize</a>
</li>
<li>
<a href="https://msdn.microsoft.com/04cb00af-f786-4548-bee3-2cc5083278c3">InitializeFromRequest</a>
</li>
<li>
<a href="https://msdn.microsoft.com/44a934f4-9ae9-4f52-9d44-f5fcf30f3837">InitializeFromTemplateName</a>
</li>
</ul>





## -see-also




<a href="https://msdn.microsoft.com/37f1dd3b-bbe9-40ab-87c9-2405d97f5541">IX509Enrollment</a>
 

 

