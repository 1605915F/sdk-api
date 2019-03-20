---
UID: NF:sdoias.ISdo.GetProperty
title: ISdo::GetProperty (sdoias.h)
author: windows-sdk-content
description: The GetProperty method retrieves the value of the specified property.
old-location: nps\SDO_isdo_getproperty.htm
tech.root: Nps
ms.assetid: 9567e731-4240-4b37-8757-2e25824bba0a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetProperty, GetProperty method [Network Policy Server], GetProperty method [Network Policy Server],ISdo interface, ISdo interface [Network Policy Server],GetProperty method, ISdo.GetProperty, ISdo::GetProperty, _sdo_isdo_getproperty, nps.SDO_isdo_getproperty, sdo.isdo_getproperty, sdoias/ISdo::GetProperty
ms.topic: method
req.header: sdoias.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: SdoIas.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Iassdo.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Iassdo.dll
api_name:
 - ISdo.GetProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISdo::GetProperty


## -description


The 
<b>GetProperty</b> method retrieves the value of the specified property.


## -parameters




### -param Id [in]

Specifies the ID of an existing property.


### -param pValue [out]

Pointer to a 
<a href="https://msdn.microsoft.com/en-us/library/ms221627(v=VS.85).aspx">VARIANT</a> that contains the value of the property.


## -returns



If the method succeeds the return value is <b>S_OK</b>.

If the method fails, the return value is one of the following error codes.




## -see-also




<a href="https://msdn.microsoft.com/9c7ee4d7-987f-45ae-810f-fc310955f36d">IASCOMMONPROPERTIES</a>



<a href="https://msdn.microsoft.com/f8f49bf2-d8cc-40ad-ac52-05d74bcd931c">ISdo</a>



<a href="https://msdn.microsoft.com/c2e440a7-d58c-4542-bd0b-a06b810edd34">ISdo::SetProperty</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221627(v=VS.85).aspx">VARIANT</a>
 

 

