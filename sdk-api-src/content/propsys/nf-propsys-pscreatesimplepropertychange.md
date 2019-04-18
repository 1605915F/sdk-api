---
UID: NF:propsys.PSCreateSimplePropertyChange
title: PSCreateSimplePropertyChange function (propsys.h)
author: windows-sdk-content
description: Creates a simple property change.
old-location: properties\PSCreateSimplePropertyChange.htm
tech.root: properties
ms.assetid: d0bec600-47bd-481c-94b2-ffdff4f2c09b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: PSCreateSimplePropertyChange, PSCreateSimplePropertyChange function [Windows Properties], _shell_PSCreateSimplePropertyChange, properties.PSCreateSimplePropertyChange, propsys/PSCreateSimplePropertyChange, shell.PSCreateSimplePropertyChange
ms.topic: function
req.header: propsys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
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
req.dll: Propsys.dll (version 6.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Propsys.dll
api_name:
 - PSCreateSimplePropertyChange
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
ms.custom: 19H1
---

# PSCreateSimplePropertyChange function


## -description


Creates a simple property change.


## -parameters




### -param flags [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb762521(v=VS.85).aspx">PKA_FLAGS</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb762521(v=VS.85).aspx">PKA_FLAGS</a> flags.


### -param key [in]

Type: <b>REFPROPERTYKEY</b>

Reference to a <a href="https://msdn.microsoft.com/en-us/library/Bb773381(v=VS.85).aspx">PROPERTYKEY</a> structure.


### -param propvar [in]

Type: <b>REFPROPVARIANT</b>

Reference to a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


### -param riid [in]

Type: <b>REFIID</b>

Reference to a specified IID.


### -param ppv [out]

Type: <b>void**</b>

The address of an <a href="https://msdn.microsoft.com/en-us/library/Bb775244(v=VS.85).aspx">IPropertyChange</a> interface pointer.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Property changes can be placed into an <a href="https://msdn.microsoft.com/en-us/library/Bb775223(v=VS.85).aspx">IPropertyChangeArray</a> which can then be used with <a href="https://msdn.microsoft.com/6596607e-0699-4eb6-b0d6-7cc2e5eb49c7">IFileOperation</a> to modify the properties on an item.



