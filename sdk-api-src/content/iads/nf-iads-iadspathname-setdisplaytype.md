---
UID: NF:iads.IADsPathname.SetDisplayType
title: IADsPathname::SetDisplayType (iads.h)
author: windows-sdk-content
description: Specifies how to display the path of an object.
old-location: adsi\iadspathname_setdisplaytype.htm
tech.root: adsi
ms.assetid: 2d975482-74f6-4ffa-a243-baa5f6a8d200
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IADsPathname interface [ADSI],SetDisplayType method, IADsPathname.SetDisplayType, IADsPathname::SetDisplayType, SetDisplayType, SetDisplayType method [ADSI], SetDisplayType method [ADSI],IADsPathname interface, _ds_iadspathname_setdisplaytype, adsi.iadspathname__setdisplaytype, adsi.iadspathname_setdisplaytype, iads/IADsPathname::SetDisplayType
ms.topic: method
req.header: iads.h
req.include-header: 
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
req.lib: 
req.dll: Activeds.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Activeds.dll
api_name:
 - IADsPathname.SetDisplayType
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IADsPathname::SetDisplayType


## -description


The <b>IADsPathname::SetDisplayType</b> method specifies how to display the path  of an object. It can query for the path to be displayed in a string with both naming attributes and values, that is, "CN=Jeff Smith" or with values only, that is, "Jeff Smith".


## -parameters




### -param lnDisplayType

The display type of a path  as defined in  <a href="https://msdn.microsoft.com/bc57aa4d-99f6-483f-b027-9b66b0c3bad1">ADS_DISPLAY_ENUM</a>.


## -returns



This method supports the standard return values, including the following:




## -see-also




<a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>



<a href="https://msdn.microsoft.com/bc57aa4d-99f6-483f-b027-9b66b0c3bad1">ADS_DISPLAY_ENUM</a>



<a href="https://msdn.microsoft.com/9aa26d6c-aa86-4a23-a986-b8cb9057772a">IADsPathname</a>
 

 

