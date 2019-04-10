---
UID: NF:iads.IADsContainer.Create
title: IADsContainer::Create (iads.h)
author: windows-sdk-content
description: Sets up a request to create a directory object of the specified schema class and a given name in the container.
old-location: adsi\iadscontainer_create.htm
tech.root: adsi
ms.assetid: 9498ef4d-7a03-487f-91a7-189f17a38a24
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Create, Create method [ADSI], Create method [ADSI],IADsContainer interface, IADsContainer interface [ADSI],Create method, IADsContainer.Create, IADsContainer::Create, _ds_iadscontainer_create, adsi.iadscontainer__create, adsi.iadscontainer_create, iads/IADsContainer::Create
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
 - IADsContainer.Create
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IADsContainer::Create


## -description


The <b>IADsContainer::Create</b> method sets up a request to create a directory object of the specified schema class and a given name in the container. The object is not made persistent until  <a href="https://msdn.microsoft.com/e7ff6acd-b7c4-463d-a34f-fd793067c63a">IADs::SetInfo</a> is called on the new object. This allows for setting mandatory properties on the new object.


## -parameters




### -param ClassName [in]

Name of the schema class object to be created. The name is that returned from the  <a href="https://msdn.microsoft.com/f53d9ee0-3f4d-4a01-b953-98d168ad94cb">IADs::get_Schema</a> property method.


### -param RelativeName [in]

Relative name of the object as it is known in the underlying directory and identical to the one retrieved through the  <a href="https://msdn.microsoft.com/f53d9ee0-3f4d-4a01-b953-98d168ad94cb">IADs::get_Name</a> property method.


### -param ppObject [out]

Indirect pointer to the  <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface on the newly created object.


## -returns



This method supports the standard return values, including S_OK for a successful operation. For more information about error codes, see  <a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/6c1d6c7c-e003-47f9-adfa-4a753fb3e9b2">IADsContainer</a>



<a href="https://msdn.microsoft.com/2f3873e0-376e-4212-a28d-bd9bc112f6cf">IADsContainer::Delete</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>
 

 

