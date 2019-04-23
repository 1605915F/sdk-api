---
UID: NF:propsys.WinRTPropertyValueToPropVariant
title: WinRTPropertyValueToPropVariant function (propsys.h)
author: windows-sdk-content
description: Copies the content from a Windows runtime property value to a PROPVARIANT structure.
old-location: properties\winrtpropertyvaluetopropvariant.htm
tech.root: properties
ms.assetid: 3D6853B0-0A3F-4ACF-9C93-478688DAE9CF
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: WinRTPropertyValueToPropVariant, WinRTPropertyValueToPropVariant function [Windows Properties], properties.winrtpropertyvaluetopropvariant, propsys/WinRTPropertyValueToPropVariant
ms.topic: function
req.header: propsys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Propsys.lib
req.dll: Propsys.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Propsys.dll
api_name:
 - WinRTPropertyValueToPropVariant
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# WinRTPropertyValueToPropVariant function


## -description


Copies the content from a Windows runtime property value to a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


## -parameters




### -param punkPropertyValue [in, optional]

A pointer to the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface from which this function can access the contents of a Windows runtime property value by retrieving and using the <a href="https://docs.microsoft.com/en-us/windows/desktop/api/windows.foundation/nn-windows-foundation-ipropertyvalue">Windows::Foundation::IPropertyValue</a> interface.


### -param ppropvar [out]

Pointer to a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure. When this function returns, the <b>PROPVARIANT</b> contains the converted info.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/38DD3673-17FD-4F2A-BA58-A1A9983B92BF">PropVariantToWinRTPropertyValue</a>
 

 

