---
UID: NF:instance.CInstance.SetCHString
title: CInstance::SetCHString (instance.h)
author: windows-sdk-content
description: The SetCHString(LPCWSTR, const CHString&) method sets a string property.
old-location: wmi\cinstance_setchstring_lpcwstr__const_chstring__.htm
tech.root: WmiSdk
ms.assetid: 590df94c-3992-49eb-a043-c5d8e1e72455
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "?SetCHString@CInstance@@QAE_NPBGABVCHString@@@Z, ?SetCHString@CInstance@@QEAA_NPEBGAEBVCHString@@@Z, CInstance interface [Windows Management Instrumentation],SetCHString method, CInstance.SetCHString, CInstance::SetCHString, CInstance::SetCHString(LPCWSTR,const CHString&), SetCHString, SetCHString method [Windows Management Instrumentation], SetCHString method [Windows Management Instrumentation],CInstance interface, instance/CInstance::SetCHString, wmi.cinstance_setchstring_lpcwstr__const_chstring__"
ms.topic: method
req.header: instance.h
req.include-header: FwCommon.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: FrameDyn.lib
req.dll: FrameDynOS.dll; FrameDyn.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - FrameDynOS.dll
 - FrameDyn.dll
api_name:
 - CInstance.SetCHString
 - ?SetCHString@CInstance@@QAE_NPBGABVCHString@@@Z
 - ?SetCHString@CInstance@@QEAA_NPEBGAEBVCHString@@@Z
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CInstance::SetCHString


## -description


<p class="CCE_Message">[The <a href="https://msdn.microsoft.com/aed29340-eb64-437d-b7e8-4f0e49c8288a">CInstance</a> class 
    is part of the WMI Provider Framework which is now considered in final state, and no further development, 
    enhancements, or updates will be available for non-security related issues affecting these libraries. The 
    <a href="https://msdn.microsoft.com/7F311E1B-5CE6-488D-9411-DE1822D95C3B">MI APIs</a> should be used for all new 
    development.]

The <b>SetCHString(LPCWSTR, const CHString&amp;)</b> method sets a string property.


## -parameters




### -param name

Name of the string property that is set.


### -param str [ref]

Value assigned to the string property.


## -returns



Returns <b>TRUE</b> if the operation was successful and <b>FALSE</b> if an attempt was made to set a nonexistent or non-string property.  More information is available in the log file, Framework.log.




## -see-also




<a href="https://msdn.microsoft.com/aed29340-eb64-437d-b7e8-4f0e49c8288a">CInstance</a>



<a href="https://msdn.microsoft.com/a75b574d-9ee7-4930-a003-5d71c5f1d687">CInstance::SetCHString</a>
 

 

