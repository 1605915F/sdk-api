---
UID: NF:ocidl.IPropertyPage.IsPageDirty
title: IPropertyPage::IsPageDirty (ocidl.h)
author: windows-sdk-content
description: Indicates whether the property page has changed since it was activated or since the most recent call to Apply.
old-location: com\ipropertypage_ispagedirty.htm
tech.root: com
ms.assetid: 6a19a659-8fab-4218-bc5a-c53860f578f6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPropertyPage interface [COM],IsPageDirty method, IPropertyPage.IsPageDirty, IPropertyPage::IsPageDirty, IsPageDirty, IsPageDirty method [COM], IsPageDirty method [COM],IPropertyPage interface, _ctrl_ipropertypage_ispagedirty, com.ipropertypage_ispagedirty, ocidl/IPropertyPage::IsPageDirty
ms.topic: method
req.header: ocidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OCIdl.idl
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
 - OCIdl.h
api_name:
 - IPropertyPage.IsPageDirty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPropertyPage::IsPageDirty


## -description


Indicates whether the property page has changed since it was activated or since the most recent call to <a href="https://msdn.microsoft.com/af0a1b49-54c3-453f-bd6a-70b63d625acb">Apply</a>.


## -parameters






## -returns



This method returns S_OK to indicate that the property page has changed. Otherwise, it returns S_FALSE.




## -remarks



The property sheet uses this information to enable or disable the <b>Apply</b> button in the dialog box. There is no need to apply the values on a property page if those values are already current with the underlying objects.

<h3><a id="Notes_to_Implementers"></a><a id="notes_to_implementers"></a><a id="NOTES_TO_IMPLEMENTERS"></a>Notes to Implementers</h3>
This method has no reason to return an error code, since the inability to determine if the page is dirty should return S_OK as a default. In this way, the user has a chance to update the values. The page should not return an error code, since an error code is not the same as S_OK and would indicate that the page is not dirty. Then, the property frame could potentially disable the <b>Apply</b> button, not allowing the user to make sure that the property values are current.




## -see-also




<a href="https://msdn.microsoft.com/ad2cb3ae-dd24-4774-95bd-f5a0773c68b1">IPropertyPage</a>
 

 

