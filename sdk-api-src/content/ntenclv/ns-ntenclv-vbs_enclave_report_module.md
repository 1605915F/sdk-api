---
UID: NS:ntenclv.VBS_ENCLAVE_REPORT_MODULE
title: VBS_ENCLAVE_REPORT_MODULE (ntenclv.h)
author: windows-sdk-content
description: Describes a module loaded for the enclave.
old-location: base\vbs_enclave_report_module.htm
tech.root: Memory
ms.assetid: FB72B01D-B3FE-4FD7-8766-B209C6BC105E
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: VBS_ENCLAVE_REPORT_MODULE, VBS_ENCLAVE_REPORT_MODULE structure, base.vbs_enclave_report_module, ntenclv/VBS_ENCLAVE_REPORT_MODULE
ms.topic: struct
req.header: ntenclv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1709 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - ntenclv.h
api_name:
 - VBS_ENCLAVE_REPORT_MODULE
product: Windows
targetos: Windows
req.typenames: VBS_ENCLAVE_REPORT_MODULE
req.redist: 
---

# VBS_ENCLAVE_REPORT_MODULE structure


## -description


Describes a module loaded for the enclave. The report contains one <b>VBS_ENCLAVE_REPORT_MODULE</b> structure for every module loaded for the enclave except the primary module for the enclave, which is described in the <b>EnclaveIdentity</b> member of the <a href="https://msdn.microsoft.com/90D6E8D2-191B-41D2-8C75-28A26462644B">VBS_ENCLAVE_REPORT</a> structure.


## -struct-fields




### -field Header

The variable data header for the report.


### -field UniqueId

The enclave unique identifier of the module.


### -field AuthorId

The author identifier of the module.


### -field FamilyId

The family identifier of the module.


### -field ImageId

The image identifier of the module.


### -field Svn

The security version number of the module.


### -field ModuleName

A NULL-terminated string that contains the name of the module as it was loaded into the enclave.


## -see-also




<a href="https://msdn.microsoft.com/90D6E8D2-191B-41D2-8C75-28A26462644B">VBS_ENCLAVE_REPORT</a>



<a href="https://msdn.microsoft.com/A0B02839-E8F4-45A1-B2BA-73E6EF9DA7C8">VBS_ENCLAVE_REPORT_VARDATA_HEADER</a>
 

 

