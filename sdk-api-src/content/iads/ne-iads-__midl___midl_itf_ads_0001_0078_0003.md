---
UID: NE:iads.__MIDL___MIDL_itf_ads_0001_0078_0003
title: "__MIDL___MIDL_itf_ads_0001_0078_0003"
author: windows-sdk-content
description: The ADS_DISPLAY_ENUM enumeration specifies how a path is to be displayed.
old-location: adsi\ads_display_enum.htm
tech.root: adsi
ms.assetid: bc57aa4d-99f6-483f-b027-9b66b0c3bad1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ADS_DISPLAY_ENUM, ADS_DISPLAY_ENUM enumeration [ADSI], ADS_DISPLAY_FULL, ADS_DISPLAY_VALUE_ONLY, __MIDL___MIDL_itf_ads_0001_0078_0003, _ds_ads_display_enum, adsi.ads__display__enum, adsi.ads_display_enum, iads/ADS_DISPLAY_ENUM, iads/ADS_DISPLAY_FULL, iads/ADS_DISPLAY_VALUE_ONLY
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Iads.h
api_name:
 - ADS_DISPLAY_ENUM
product: Windows
targetos: Windows
req.typenames: ADS_DISPLAY_ENUM
req.redist: 
---

# __MIDL___MIDL_itf_ads_0001_0078_0003 enumeration


## -description


The <b>ADS_DISPLAY_ENUM</b> enumeration specifies how a path is to be displayed.


## -enum-fields




### -field ADS_DISPLAY_FULL

The path  is displayed with both attributes and values. For example, CN=Jeff Smith.


### -field ADS_DISPLAY_VALUE_ONLY

The path is displayed with values only. For example, Jeff Smith.


## -remarks



This enumeration is used in  <a href="https://msdn.microsoft.com/2d975482-74f6-4ffa-a243-baa5f6a8d200">IADsPathname::SetDisplayType</a> method to specify how a path  is to be displayed.

<div class="alert"><b>Note</b>  Because VBScript cannot read data from a type library, VBScript applications do not understand the symbolic constants as defined above. You should use the numeric constants instead to set the appropriate flags in your VBScript applications. If you want to use the symbolic constants as a good programming practice, you should create explicit declarations of such constants, as done here, in your VBScript applications.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/f0ad5ce5-742d-40dc-ac5a-31d779e40bfd">ADSI Enumerations</a>



<a href="https://msdn.microsoft.com/2d975482-74f6-4ffa-a243-baa5f6a8d200">IADsPathname::SetDisplayType</a>
 

 

