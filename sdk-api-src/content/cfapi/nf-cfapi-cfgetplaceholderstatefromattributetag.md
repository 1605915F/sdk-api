---
UID: NF:cfapi.CfGetPlaceholderStateFromAttributeTag
title: CfGetPlaceholderStateFromAttributeTag function
author: windows-sdk-content
description: Gets a set of placeholder states based on the FileAttributes and ReparseTag values of the file.
old-location: cloudapi\cfgetplaceholderstatefromattributetag.htm
tech.root: cfApi
ms.assetid: D7B4FB60-3388-489F-9F55-153B53BBDA9F
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CfGetPlaceholderStateFromAttributeTag, CfGetPlaceholderStateFromAttributeTag function, cfapi/CfGetPlaceholderStateFromAttributeTag, cloudApi.cfgetplaceholderstatefromattributetag
ms.topic: function
req.header: cfapi.h
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
req.lib: CldApi.lib
req.dll: CldApi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - CldApi.dll
api_name:
 - CfGetPlaceholderStateFromAttributeTag
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CfGetPlaceholderStateFromAttributeTag function


## -description


Gets a set of placeholder states based on the <i>FileAttributes</i> and <i>ReparseTag</i> values of the file.


## -parameters




### -param FileAttributes [in]

The file attribute information.


### -param ReparseTag [in]

The reparse tag information from a file.


## -returns



Can include <a href="https://msdn.microsoft.com/5E814458-2045-4CFD-90AC-F1F53DEB4FD0">CF_PLACEHOLDER_STATE</a>; The placeholder state.




## -remarks



The <i>FileAttributes</i> and <i>ReparseTag</i> can be obtained by listing the directory containing the file or by directly querying <i>FileAttributeTagInfo</i> on the file.



