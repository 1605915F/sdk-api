---
UID: NF:tom.ITextStory.SetProperty
title: ITextStory::SetProperty (tom.h)
author: windows-sdk-content
description: Sets the value of the specified property.
old-location: controls\itextstory_setproperty.htm
tech.root: Controls
ms.assetid: 432afe58-a1ed-45aa-b018-bf608bbb7e2a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITextStory interface [Windows Controls],SetProperty method, ITextStory.SetProperty, ITextStory::SetProperty, SetProperty, SetProperty method [Windows Controls], SetProperty method [Windows Controls],ITextStory interface, controls.itextstory_setproperty, tom/ITextStory::SetProperty
ms.topic: method
req.header: tom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tom.idl
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
 - COM
api_location:
 - tom.h
api_name:
 - ITextStory.SetProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITextStory::SetProperty


## -description


Sets the value of the specified property.


## -parameters




### -param Type [in]

Type: <b>long</b>

The Microsoft accountID that identifies the property. Currently, no extra properties are defined.


### -param Value [in]

Type: <b>long</b>

The new property value.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the method succeeds, it returns <b>NOERROR</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/8b52c6e8-c250-4cfb-979e-770df9f94010">ITextStory</a>



<a href="https://msdn.microsoft.com/1c24e9d8-c737-42f8-87d9-585b0054b6df">ITextStory::GetProperty</a>
 

 

