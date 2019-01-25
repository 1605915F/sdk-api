---
UID: NF:termmgr.ITPluggableTerminalClassRegistration.get_Name
title: ITPluggableTerminalClassRegistration::get_Name
author: windows-sdk-content
description: The get_Name method gets the terminal's friendly name.
old-location: tapi3\itpluggableterminalclassregistration_get_name.htm
tech.root: Tapi
ms.assetid: 0bbc0862-41d7-40cc-9b9d-57a2238122ee
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITPluggableTerminalClassRegistration interface [TAPI 2.2],get_Name method, ITPluggableTerminalClassRegistration.get_Name, ITPluggableTerminalClassRegistration::get_Name, _tapi3_itpluggableterminalclassregistration_get_name, get_Name, get_Name method [TAPI 2.2], get_Name method [TAPI 2.2],ITPluggableTerminalClassRegistration interface, tapi3.itpluggableterminalclassregistration_get_name, termmgr/ITPluggableTerminalClassRegistration::get_Name
ms.topic: method
req.header: termmgr.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITPluggableTerminalClassRegistration.get_Name
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITPluggableTerminalClassRegistration::get_Name


## -description


The 
<b>get_Name</b> method gets the terminal's friendly name.


## -parameters




### -param pName [out]

The <b>BSTR</b> representation of the friendly name. The <b>BSTR</b> is allocated using 
<a href="https://msdn.microsoft.com/en-us/library/ms221458(v=VS.85).aspx">SysAllocString</a>. The <b>BSTR</b> argument should be deallocated by the client.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/178824f5-9dda-4e8a-b921-f2c9d064a83c">ITPluggableTerminalClassRegistration</a>



<a href="https://msdn.microsoft.com/d3d6c585-5592-4ed9-80bb-a55ff151edd1">put_Name</a>
 

 

