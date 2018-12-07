---
UID: NF:tuner.IEnumComponents.Next
title: IEnumComponents::Next
author: windows-sdk-content
description: The Next method retrieves the next n elements in the collection.
old-location: mstv\ienumcomponents_next.htm
tech.root: mstv
ms.assetid: 73cb45c7-1f74-46cf-a410-ec1d5fed4271
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumComponents interface [Microsoft TV Technologies],Next method, IEnumComponents.Next, IEnumComponents::Next, IEnumComponentsNext, Next, Next method [Microsoft TV Technologies], Next method [Microsoft TV Technologies],IEnumComponents interface, mstv.ienumcomponents_next, tuner/IEnumComponents::Next
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
 - tuner.h
api_name:
 - IEnumComponents.Next
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumComponents::Next


## -description



The <b>Next</b> method retrieves the next <i>n</i> elements in the collection.




## -parameters




### -param celt [in]

The number of elements to retrieve.


### -param rgelt [out]

Address of an array of <a href="https://msdn.microsoft.com/516b30ba-4f55-49b7-8085-d436bf4a94e1">IComponent</a> interface pointers that will receive the retrieved <a href="https://msdn.microsoft.com/a164cebb-92e2-4d20-a5b9-878998977971">Component</a> objects.


### -param pceltFetched [out]

Receives the number of elements actually retrieved.


## -returns



Returns S_OK if successful. If the method fails, error information can be retrieved using the standard COM <b>IErrorInfo</b> interface.




## -see-also




<a href="https://msdn.microsoft.com/8811021c-8c14-4be6-8802-76b942bb34d8">IEnumComponents Interface</a>
 

 

