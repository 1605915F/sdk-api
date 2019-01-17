---
UID: NC:d2d1effectauthor.PD2D1_PROPERTY_GET_FUNCTION
title: PD2D1_PROPERTY_GET_FUNCTION
author: windows-sdk-content
description: Gets a property from an effect.
old-location: direct2d\pd2d1_property_get_function.htm
tech.root: Direct2D
ms.assetid: A6F6F22A-762A-4D77-8008-8226C75AD205
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PD2D1_PROPERTY_GET_FUNCTION, PD2D1_PROPERTY_GET_FUNCTION function, PD2D1_PROPERTY_GET_FUNCTION function pointer [Direct2D], d2d1effectauthor/PD2D1_PROPERTY_GET_FUNCTION, direct2d.pd2d1_property_get_function
ms.topic: callback
req.header: d2d1effectauthor.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - UserDefined
api_location:
 - D2d1effectauthor.h
api_name:
 - PD2D1_PROPERTY_GET_FUNCTION
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PD2D1_PROPERTY_GET_FUNCTION callback function


## -description


Gets a property from an effect.


## -parameters




### -param *effect [in]

A pointer to the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface for the effect on which the property will be retrieved.


### -param *data [out]

A pointer to a variable that stores the data that this function retrieves on the property.


### -param dataSize

The number of bytes in the property to retrieve.


### -param *actualSize [out, optional]

A optional pointer to a variable that stores the actual number of bytes retrieved on the property. If not used, set to <b>NULL</b>.


## -returns



Returns S_OK if successful; otherwise, returns an <b>HRESULT</b> error code.




## -remarks



Supply a <b>PD2D1_PROPERTY_GET_FUNCTION</b> to the <b>getFunction</b> member of a <a href="https://msdn.microsoft.com/0eb6d428-cb65-4738-9cf3-64038b728004">D2D1_PROPERTY_BINDING</a> structure to specify the function that Direct2D uses to get data for a property.




## -see-also




<a href="https://msdn.microsoft.com/0eb6d428-cb65-4738-9cf3-64038b728004">D2D1_PROPERTY_BINDING</a>
 

 

