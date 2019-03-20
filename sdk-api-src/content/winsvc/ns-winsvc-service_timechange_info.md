---
UID: NS:winsvc._SERVICE_TIMECHANGE_INFO
title: SERVICE_TIMECHANGE_INFO (winsvc.h)
author: windows-sdk-content
description: Contains system time change settings.
old-location: base\service_timechange_info.htm
tech.root: Services
ms.assetid: 452b0678-dfea-4128-9236-273323b519f0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSERVICE_TIMECHANGE_INFO, PSERVICE_TIMECHANGE_INFO, PSERVICE_TIMECHANGE_INFO structure pointer, SERVICE_TIMECHANGE_INFO, SERVICE_TIMECHANGE_INFO structure, base.service_timechange_info, winsvc/PSERVICE_TIMECHANGE_INFO, winsvc/SERVICE_TIMECHANGE_INFO"
ms.topic: struct
req.header: winsvc.h
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
 - winsvc.h
api_name:
 - SERVICE_TIMECHANGE_INFO
product: Windows
targetos: Windows
req.typenames: SERVICE_TIMECHANGE_INFO, *PSERVICE_TIMECHANGE_INFO
req.redist: 
---

# SERVICE_TIMECHANGE_INFO structure


## -description


Contains system time change settings. 


## -struct-fields




### -field liNewTime

The new system time. 


### -field liOldTime

The previous system time. 


## -remarks



The time values in the <i>liNewTime</i> and <i>liOldTime</i> members cannot be used directly with the time functions, which typically require a <a href="https://msdn.microsoft.com/9baf8a0e-59e3-4fbd-9616-2ec9161520d1">FILETIME</a> or <a href="https://msdn.microsoft.com/f77cdf86-0f97-4a89-b565-95b46fa7d65b">SYSTEMTIME</a> structure. Convert the  <a href="https://msdn.microsoft.com/6a2985b6-5baf-49ab-af28-67c1374557ea">LARGE_INTEGER</a> structure to a  <a href="https://msdn.microsoft.com/83a10c12-2cd1-449a-af3f-b2138fc50ee0">ULARGE_INTEGER</a> structure, copy the <b>ULARGE_INTEGER</b> structure to a <b>FILETIME</b> structure, and then if necessary use the <a href="https://msdn.microsoft.com/d1d55f1f-4daa-4b9d-9962-873e38b1e0cf">FileTimeToSystemTime</a> function to convert the <b>FILETIME</b> structure to a <b>SYSTEMTIME</b> structure. 




## -see-also




<a href="https://msdn.microsoft.com/6e5b79ed-52e1-460e-b076-01afbd08775c">ChangeServiceConfig2</a>



<a href="https://msdn.microsoft.com/cb090e59-aeff-4420-bb7c-912a4911006f">QueryServiceConfig2</a>
 

 

