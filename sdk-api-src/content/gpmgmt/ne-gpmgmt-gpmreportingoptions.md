---
UID: NE:gpmgmt.__MIDL___MIDL_itf_gpmgmt_0000_0000_0008
title: GPMReportingOptions (gpmgmt.h)
author: windows-sdk-content
description: Options for Group Policy Management Console reports.
old-location: gpmc\gpmreportingoptions.htm
tech.root: gpmc
ms.assetid: 52d51058-d5fd-4b62-9206-2dc60a3eafb1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GPMReportingOptions, GPMReportingOptions enumeration [GPMC], gpmc.gpmreportingoptions, gpmgmt/GPMReportingOptions, gpmgmt/opReportComments, gpmgmt/opReportLegacy, opReportComments, opReportLegacy
ms.topic: enum
req.header: gpmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Gpmgmt.idl
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
 - gpmgmt.h
api_name:
 - GPMReportingOptions
product: Windows
targetos: Windows
req.typenames: GPMReportingOptions
req.redist: 
---

# GPMReportingOptions enumeration


## -description


<b>GPMReportingOptions</b> defines options for Group Policy Management Console  reports.

<b>GPMReportingOptions</b> defines options for Group Policy Management Console reports.

```cpp
typedef enum {
        opReportLegacy = 0,
        opReportComments = 1,
        } GPMReportingOptions;
```



## -enum-fields




### -field opReportLegacy

Use administrative template ADM files.


### -field opReportComments

Include comments.

