---
UID: NS:winnt._JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION
title: JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION
author: windows-sdk-content
description: Contains basic accounting and I/O accounting information for a job object.
old-location: base\jobobject_basic_and_io_accounting_information_str.htm
tech.root: procthread
ms.assetid: 5c3e4002-d4d2-4a8c-ab0c-f6bcdd62947a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PJOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION, JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION, JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION structure, PJOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION, PJOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION structure pointer, _JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION, _win32_jobobject_basic_and_io_accounting_information_str, base.jobobject_basic_and_io_accounting_information_str, winnt/JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION, winnt/PJOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION"
ms.topic: struct
req.header: winnt.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - WinNT.h
api_name:
 - JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION
product: Windows
targetos: Windows
req.typenames: JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION, *PJOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION
req.redist: 
---

# JOBOBJECT_BASIC_AND_IO_ACCOUNTING_INFORMATION structure


## -description


Contains basic accounting and I/O accounting information for a job object.


## -struct-fields




### -field BasicInfo

A 
<a href="https://msdn.microsoft.com/84dbe191-a5bf-4f55-815f-c4f2e60da22b">JOBOBJECT_BASIC_ACCOUNTING_INFORMATION</a> structure that specifies the basic accounting information for the job.


### -field IoInfo

An 
<a href="https://msdn.microsoft.com/78729cbe-5256-4939-a7cc-c393662f8361">IO_COUNTERS</a> structure that specifies the I/O accounting information for the job. The structure includes information for all processes that have ever been associated with the job, in addition to the information for all processes currently associated with the job.


## -see-also




<a href="https://msdn.microsoft.com/78729cbe-5256-4939-a7cc-c393662f8361">IO_COUNTERS</a>



<a href="https://msdn.microsoft.com/84dbe191-a5bf-4f55-815f-c4f2e60da22b">JOBOBJECT_BASIC_ACCOUNTING_INFORMATION</a>



<a href="https://msdn.microsoft.com/d843d578-fd67-4708-959f-00245ff70ec6">QueryInformationJobObject</a>
 

 

