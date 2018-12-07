---
UID: NS:documenttarget.__MIDL___MIDL_itf_documenttarget_0000_0001_0001
title: "__MIDL___MIDL_itf_documenttarget_0000_0001_0001"
author: windows-sdk-content
description: Defines a payload to be used by the PackageStatusUpdated method. This structure is a generic version of XPS_JOB_STATUS.
old-location: xps\printdocumentpackagestatus.htm
tech.root: printdocs
ms.assetid: A499CB8D-B2E3-4343-A9AF-079C75EF1441
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PPrintDocumentPackageStatus, PPrintDocumentPackageStatus structure pointer [XPS Documents and Packaging], PrintDocumentPackageStatus, PrintDocumentPackageStatus structure [XPS Documents and Packaging], __MIDL___MIDL_itf_documenttarget_0000_0001_0001, documenttarget/PPrintDocumentPackageStatus, documenttarget/PrintDocumentPackageStatus, xps.printdocumentpackagestatus
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: documenttarget.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - Documenttarget.h
api_name:
 - PrintDocumentPackageStatus
product: Windows
targetos: Windows
req.typenames: PrintDocumentPackageStatus
req.redist: 
---

# __MIDL___MIDL_itf_documenttarget_0000_0001_0001 structure


## -description


Defines a payload to be used by the <a href="https://msdn.microsoft.com/A672E554-B117-475C-A01E-9FD4EA31621E">PackageStatusUpdated</a> method. This structure is a generic version of XPS_JOB_STATUS.


## -struct-fields




### -field JobId

The job ID.


### -field CurrentDocument

The zero-based index of the most recently processed document.


### -field CurrentPage

The zero-based index of the most recently processed page in the current document


### -field CurrentPageTotal

A running total of the number of pages that have been processed by the print job.


### -field Completion

The completion status of the job.


### -field PackageStatus

The error state of the job.


## -see-also




<a href="https://msdn.microsoft.com/A672E554-B117-475C-A01E-9FD4EA31621E">PackageStatusUpdated</a>
 

 

