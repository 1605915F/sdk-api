---
UID: NF:fsrmreports.IFsrmFileManagementJob.get_PropertyConditions
title: IFsrmFileManagementJob::get_PropertyConditions
author: windows-sdk-content
description: A list of property conditions specified for the job.
old-location: fsrm\ifsrmfilemanagementjob_propertyconditions.htm
tech.root: fsrm
ms.assetid: 49435c4b-211e-4aae-a6b3-ad40de811526
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFsrmFileManagementJob interface [File Server Resource Manager],PropertyConditions property, IFsrmFileManagementJob.PropertyConditions, IFsrmFileManagementJob.get_PropertyConditions, IFsrmFileManagementJob::PropertyConditions, IFsrmFileManagementJob::get_PropertyConditions, PropertyConditions property [File Server Resource Manager], PropertyConditions property [File Server Resource Manager],IFsrmFileManagementJob interface, fs.ifsrmfilemanagementjob_propertyconditions, fsrm.ifsrmfilemanagementjob_propertyconditions, fsrmreports/IFsrmFileManagementJob::PropertyConditions, fsrmreports/IFsrmFileManagementJob::get_PropertyConditions, get_PropertyConditions
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: fsrmreports.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2
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
req.dll: SrmSvc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - SrmSvc.dll
api_name:
 - IFsrmFileManagementJob.PropertyConditions
 - IFsrmFileManagementJob.get_PropertyConditions
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFsrmFileManagementJob::get_PropertyConditions


## -description


<p class="CCE_Message">[This property is supported for compatibility but it's recommended to use the 
    <a href="https://msdn.microsoft.com/1CE772FA-CE33-4900-A499-058175A7C37E">FSRM WMI Classes</a> to manage FSRM. Please see the 
    <a href="https://msdn.microsoft.com/1ce33602-0ada-4d82-aebb-9dee7dc8b2f3">MSFT_FSRMFileManagementJob</a> class.]

A list of property conditions specified for the job.

This property is read-only.


## -parameters


## -remarks



To specify a property condition for the job, call the 
    <a href="https://msdn.microsoft.com/1b264e9c-4ba0-4de2-acdc-94338519c5af">IFsrmFileManagementJob::CreatePropertyCondition</a> 
    method.




## -see-also




<a href="https://msdn.microsoft.com/e9ae697d-4f7c-47d9-8d2a-c46c2e5f838f">IFsrmFileManagementJob</a>



<a href="https://msdn.microsoft.com/1ce33602-0ada-4d82-aebb-9dee7dc8b2f3">MSFT_FSRMFileManagementJob</a>
 

 

