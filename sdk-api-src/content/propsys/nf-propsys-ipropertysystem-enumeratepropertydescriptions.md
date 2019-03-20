---
UID: NF:propsys.IPropertySystem.EnumeratePropertyDescriptions
title: IPropertySystem::EnumeratePropertyDescriptions (propsys.h)
author: windows-sdk-content
description: Gets an instance of the subsystem object that implements IPropertyDescriptionList, to obtain either the entire or a partial list of property descriptions in the system.
old-location: properties\IPropertySystem_EnumeratePropertyDescriptions.htm
tech.root: properties
ms.assetid: eb87e6b6-2a48-497a-8a42-9c929a742502
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnumeratePropertyDescriptions, EnumeratePropertyDescriptions method [Windows Properties], EnumeratePropertyDescriptions method [Windows Properties],IPropertySystem interface, IPropertySystem interface [Windows Properties],EnumeratePropertyDescriptions method, IPropertySystem.EnumeratePropertyDescriptions, IPropertySystem::EnumeratePropertyDescriptions, properties.IPropertySystem_EnumeratePropertyDescriptions, propsys/IPropertySystem::EnumeratePropertyDescriptions, shell.IPropertySystem_EnumeratePropertyDescriptions, shell_IPropertySystem_EnumeratePropertyDescriptions
ms.topic: method
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
req.dll: Propsys.dll (version 5.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Propsys.dll
api_name:
 - IPropertySystem.EnumeratePropertyDescriptions
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# IPropertySystem::EnumeratePropertyDescriptions


## -description


Gets an instance of the subsystem object that implements <a href="https://msdn.microsoft.com/en-us/library/Bb761511(v=VS.85).aspx">IPropertyDescriptionList</a>, to obtain either the entire or a partial list of property descriptions in the system.


## -parameters




### -param filterOn [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb762524(v=VS.85).aspx">PROPDESC_ENUMFILTER</a></b>

The list to return. See <a href="https://msdn.microsoft.com/en-us/library/Bb762524(v=VS.85).aspx">PROPDESC_ENUMFILTER</a>. Valid values for this method are 0 through 4.


### -param riid [in]

Type: <b>REFIID</b>

A reference to the desired IID.


### -param ppv [out]

Type: <b>void**</b>

The address of an <a href="https://msdn.microsoft.com/en-us/library/Bb761511(v=VS.85).aspx">IPropertyDescriptionList</a> interface pointer.


## -returns



Type: <b>HRESULT</b>

Returns one of the following values.

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
Indicates interface is obtained.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Indicates <i>ppv</i> is <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



This method is not implemented where BUILDING_DOWNLEVEL_LIB is defined.

It is recommended that you use the IID_PPV_ARGS macro, defined in objbase.h, to package the <i>riid</i> and <i>ppv</i> parameters. This macro provides the correct IID based on the interface pointed to by the value in <i>ppv</i>, eliminating the possibility of a coding error.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb761437(v=VS.85).aspx">IPropertySystem</a>
 

 

