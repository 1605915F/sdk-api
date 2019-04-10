---
UID: NN:propsys.IPropertySystem
title: IPropertySystem (propsys.h)
author: windows-sdk-content
description: Exposes methods that get property descriptions, register and unregister property schemas, enumerate property descriptions, and format property values in a type-strict way.
old-location: properties\IPropertySystem.htm
tech.root: properties
ms.assetid: 9ead94d9-4d4e-44c6-8c53-11c4c4ee2fb2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IPropertySystem, IPropertySystem interface [Windows Properties], IPropertySystem interface [Windows Properties],described, properties.IPropertySystem, propsys/IPropertySystem, shell.IPropertySystem, shell_IPropertySystem
ms.topic: interface
req.header: propsys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Propsys.idl
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
 - Propsys.h
api_name:
 - IPropertySystem
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# IPropertySystem interface


## -description


Exposes methods that get property descriptions, register and unregister property schemas, enumerate property descriptions, and format property values in a type-strict way.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IPropertySystem</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IPropertySystem</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IPropertySystem</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761426(v=VS.85).aspx">EnumeratePropertyDescriptions</a>
</td>
<td align="left" width="63%">
Gets an instance of the subsystem object that implements <a href="https://msdn.microsoft.com/en-us/library/Bb761511(v=VS.85).aspx">IPropertyDescriptionList</a>, to obtain either the entire or a partial list of property descriptions in the system.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761521(v=VS.85).aspx">FormatForDisplay</a>
</td>
<td align="left" width="63%">
Gets a formatted, Unicode string representation of a property value.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761430(v=VS.85).aspx">FormatForDisplayAlloc</a>
</td>
<td align="left" width="63%">
Gets a string representation of a property value to an allocated memory buffer.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761432(v=VS.85).aspx">GetPropertyDescription</a>
</td>
<td align="left" width="63%">
Gets an instance of the subsystem object that implements <a href="https://msdn.microsoft.com/en-us/library/Bb761561(v=VS.85).aspx">IPropertyDescription</a>, to obtain the property description for a given <a href="https://msdn.microsoft.com/en-us/library/Bb773381(v=VS.85).aspx">PROPERTYKEY</a>.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761434(v=VS.85).aspx">GetPropertyDescriptionByName</a>
</td>
<td align="left" width="63%">
Gets an instance of the subsystem object that implements <a href="https://msdn.microsoft.com/en-us/library/Bb761561(v=VS.85).aspx">IPropertyDescription</a>, to obtain the property description for a given canonical name.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761436(v=VS.85).aspx">GetPropertyDescriptionListFromString</a>
</td>
<td align="left" width="63%">
Gets an instance of the subsystem object that implements <a href="https://msdn.microsoft.com/en-us/library/Bb761511(v=VS.85).aspx">IPropertyDescriptionList</a>, to obtain an ordered collection of property descriptions, based on the provided string.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761439(v=VS.85).aspx">RefreshPropertySchema</a>
</td>
<td align="left" width="63%">
Not currently supported.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761441(v=VS.85).aspx">RegisterPropertySchema</a>
</td>
<td align="left" width="63%">
Informs the schema subsystem of the addition of a property description schema file.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Bb761445(v=VS.85).aspx">UnregisterPropertySchema</a>
</td>
<td align="left" width="63%">
Informs the schema subsystem of the removal of a property description schema (.propdesc) file, using a file path to the .propdesc file on the local machine.

</td>
</tr>
</table> 


## -remarks



Many of the exported APIs (such as <a href="https://msdn.microsoft.com/en-us/library/Bb776503(v=VS.85).aspx">PSGetPropertyDescription</a>) are simply wrappers around the <a href="https://msdn.microsoft.com/en-us/library/Bb761437(v=VS.85).aspx">IPropertySystem</a> methods. If your code calls a lot of these helper APIs in sequence, it may be worthwhile to instantiate a single <b>IPropertySystem</b> object, and call the methods directly, rather than calling the helper APIs. (To improve the performance, the helper APIs do obtain a cached instance of the <b>IPropertySystem</b> object.)



