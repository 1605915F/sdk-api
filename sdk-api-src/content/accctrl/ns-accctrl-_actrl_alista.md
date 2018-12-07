---
UID: NS:accctrl._ACTRL_ALISTA
title: "_ACTRL_ALISTA"
author: windows-sdk-content
description: Contains an array of access-control lists for an object and its properties.
old-location: com\actrl_access.htm
tech.root: com
ms.assetid: d7fb10c1-ebb8-44cf-b61c-a70a787b324f
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: "*PACTRL_ACCESSA, *PACTRL_AUDITA, ACTRL_ACCESS, ACTRL_ACCESS structure [COM], ACTRL_ACCESSA, ACTRL_ACCESSW, ACTRL_AUDIT, ACTRL_AUDITA, PACTRL_ACCESS, PACTRL_ACCESS structure pointer [COM], PACTRL_ACCESSW_ALLOCATE_ALL_NODES, _ACTRL_ALISTA, _ACTRL_ALISTW, accctrl/ACTRL_ACCESS, accctrl/ACTRL_ACCESSA, accctrl/ACTRL_ACCESSW, accctrl/PACTRL_ACCESS, com.actrl_access"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: accctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: ACTRL_ACCESSW (Unicode) and ACTRL_ACCESSA (ANSI)
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
 - HeaderDef
api_location:
 - AccCtrl.h
api_name:
 - ACTRL_ACCESS
 - ACTRL_ACCESSA
 - ACTRL_ACCESSW
product: Windows
targetos: Windows
req.typenames: ACTRL_ACCESSA, *PACTRL_ACCESSA, ACTRL_AUDITA, *PACTRL_AUDITA
req.redist: 
---

# _ACTRL_ALISTA structure


## -description


Contains an array of access-control lists for an object and its properties.


## -struct-fields




### -field cEntries

The number of entries in the <b>pPropertyAccessList</b> array.


### -field pPropertyAccessList

An array of <a href="https://msdn.microsoft.com/90b13dd1-0ca6-4674-b9fa-a61aed4637d7">ACTRL_PROPERTY_ENTRY</a> structures. Each structure contains a list of access-control entries for an object or a specified property on the object.


### -field pPropertyAccessList.size_is

 


### -field pPropertyAccessList.size_is.cEntries

 




## -remarks



Note the following type definition.

<pre class="syntax" xml:space="preserve"><code>typedef PACTRL_ACCESSW PACTRL_ACCESSW_ALLOCATE_ALL_NODES;</code></pre>



## -see-also




<a href="https://msdn.microsoft.com/f8ec6743-633b-4c79-afac-68eb20e07b2a">IAccessControl::GrantAccessRights</a>
 

 

