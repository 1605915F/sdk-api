---
UID: NF:msinkaut.IInkExtendedProperties.Clear
title: IInkExtendedProperties::Clear (msinkaut.h)
author: windows-sdk-content
description: Clears all of the IInkExtendedProperty objects from the IInkExtendedProperties collection.
old-location: tablet\iinkextendedproperties_clear.htm
tech.root: tablet
ms.assetid: b5270e5c-51fa-4d1f-b4e0-9129c61bac88
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Clear, Clear method [Tablet PC], Clear method [Tablet PC],IInkExtendedProperties interface, IInkExtendedProperties interface [Tablet PC],Clear method, IInkExtendedProperties.Clear, IInkExtendedProperties::Clear, b5270e5c-51fa-4d1f-b4e0-9129c61bac88, msinkaut/IInkExtendedProperties::Clear, tablet.iinkextendedproperties_clear
ms.topic: method
req.header: msinkaut.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: InkObj.dll
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - InkObj.dll
 - InkObj.dll.dll
api_name:
 - IInkExtendedProperties.Clear
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInkExtendedProperties::Clear


## -description



Clears all of the <a href="https://msdn.microsoft.com/53146f37-343a-4886-a0bb-d76d50ca96ba">IInkExtendedProperty</a> objects from the <a href="https://msdn.microsoft.com/c7b7f40f-0c28-4848-83d6-d5db73eef998">IInkExtendedProperties</a> collection.




## -parameters






## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INK_EXCEPTION</b></dt>
</dl>
</td>
<td width="60%">
An exception occurred inside the method.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unspecified error occurred.

</td>
</tr>
</table>
 




## -remarks



To clear only one extended property at a time, call the <a href="https://msdn.microsoft.com/2211a462-df26-4168-b89c-9607683defdb">Remove</a> method of the <a href="https://msdn.microsoft.com/c7b7f40f-0c28-4848-83d6-d5db73eef998">IInkExtendedProperties</a> collection.




## -see-also




<a href="https://msdn.microsoft.com/c7b7f40f-0c28-4848-83d6-d5db73eef998">IInkExtendedProperties Interface</a>



<a href="https://msdn.microsoft.com/2211a462-df26-4168-b89c-9607683defdb">Remove Method [IInkExtendedProperties Interface]</a>
 

 

