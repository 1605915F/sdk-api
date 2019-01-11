---
UID: NF:fhcfg.IFhConfigMgr.ValidateTarget
title: IFhConfigMgr::ValidateTarget
author: windows-sdk-content
description: Checks whether a certain storage device or network share can be used as a File History backup target.
old-location: winprog\ifhconfigmgr_validatetarget.htm
tech.root: DevNotes
ms.assetid: EC41C4EE-A909-4DD4-AA32-5054BBEAF421
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FhConfigMgr class [Windows API],ValidateTarget method, IFhConfigMgr interface [Windows API],ValidateTarget method, IFhConfigMgr.ValidateTarget, IFhConfigMgr::ValidateTarget, ValidateTarget, ValidateTarget method [Windows API], ValidateTarget method [Windows API],FhConfigMgr class, ValidateTarget method [Windows API],IFhConfigMgr interface, fhcfg/IFhConfigMgr::ValidateTarget, winprog.ifhconfigmgr_validatetarget
ms.topic: method
req.header: fhcfg.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Fhcfg.idl
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
 - COM
api_location:
 - Fhcfg.h
api_name:
 - IFhConfigMgr.ValidateTarget
 - FhConfigMgr.ValidateTarget
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFhConfigMgr::ValidateTarget


## -description


 Checks whether a certain storage device or network share can be used as a File History backup target.


## -parameters




### -param TargetUrl [in]

The storage device or network share to be validated.


### -param ValidationResult [out]

Receives the result of the device validation. See the <a href="https://msdn.microsoft.com/DAADC244-D0F5-44F9-9F61-48E6C6EFB91A">FH_DEVICE_VALIDATION_RESULT</a> enumeration for the list of possible device validation result values.


## -returns



<b>S_OK</b> on success, or an unsuccessful <b>HRESULT</b> value on failure. Possible unsuccessful <b>HRESULT</b> values include values defined in the FhErrors.h header file.




## -remarks



For local disks, the <i>TargetUrl</i> parameter contains the drive letter. This path must end with a trailing backslash (for example, "X:\").

For network shares, the <i>TargetUrl</i> parameter contains the full path of the share.  This path must end with a trailing backslash (for example, "\\myserver\myshare\").




## -see-also




<a href="https://msdn.microsoft.com/CC97FC0F-3AA4-4D8A-81B3-14F68FDF5788">FhConfigMgr</a>



<a href="https://msdn.microsoft.com/CDE8A011-6E78-49DF-A5E1-8E968355BA11">IFhConfigMgr</a>



<a href="https://msdn.microsoft.com/570CB5FD-7586-41AD-84A6-DA6966B18E91">IFhConfigMgr::GetDefaultTarget</a>
 

 

