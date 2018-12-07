---
UID: NF:vsmgmt.IVssEnumMgmtObject.Clone
title: IVssEnumMgmtObject::Clone
author: windows-sdk-content
description: Creates a copy of the specified list of enumerated elements by creating a copy of the IVssEnumMgmtObject enumerator object.
old-location: base\ivssenummgmtobject_clone.htm
tech.root: vss
ms.assetid: f957052a-5511-4f00-b864-1f03ead2ba58
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Clone, Clone method [VSS], Clone method [VSS],IVssEnumMgmtObject interface, IVssEnumMgmtObject interface [VSS],Clone method, IVssEnumMgmtObject.Clone, IVssEnumMgmtObject::Clone, base.ivssenummgmtobject_clone, vsmgmt/IVssEnumMgmtObject::Clone
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: vsmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - VsMgmt.h
api_name:
 - IVssEnumMgmtObject.Clone
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVssEnumMgmtObject::Clone


## -description


The <b>Clone</b> method creates a copy of the 
    specified list of enumerated elements by creating a copy of the 
    <a href="https://msdn.microsoft.com/c2067822-1824-4676-8376-7d83fcbbaea3">IVssEnumMgmtObject</a> enumerator object.


## -parameters




### -param ppenum [in, out]

Address of an <a href="https://msdn.microsoft.com/c2067822-1824-4676-8376-7d83fcbbaea3">IVssEnumMgmtObject</a> interface 
      pointer. Set the value of this parameter to <b>NULL</b> before calling this method.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/c2067822-1824-4676-8376-7d83fcbbaea3">IVssEnumMgmtObject</a>
 

 

