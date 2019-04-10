---
UID: NF:tapi3if.ITPluggableTerminalClassInfo.get_TerminalClass
title: ITPluggableTerminalClassInfo::get_TerminalClass (tapi3if.h)
author: windows-sdk-content
description: The get_TerminalClass method gets the terminal's terminal class.
old-location: tapi3\itpluggableterminalclassinfo_get_terminalclass.htm
tech.root: Tapi
ms.assetid: 7dfa6cf8-23b8-4959-ba39-6efda1d71562
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITPluggableTerminalClassInfo interface [TAPI 2.2],get_TerminalClass method, ITPluggableTerminalClassInfo.get_TerminalClass, ITPluggableTerminalClassInfo::get_TerminalClass, _tapi3_itpluggableterminalclassinfo_get_terminalclass, get_TerminalClass, get_TerminalClass method [TAPI 2.2], get_TerminalClass method [TAPI 2.2],ITPluggableTerminalClassInfo interface, tapi3.itpluggableterminalclassinfo_get_terminalclass, tapi3if/ITPluggableTerminalClassInfo::get_TerminalClass
ms.topic: method
req.header: tapi3if.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITPluggableTerminalClassInfo.get_TerminalClass
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITPluggableTerminalClassInfo::get_TerminalClass


## -description


The 
<b>get_TerminalClass</b> method gets the terminal's terminal class.


## -parameters




### -param pTerminalClass [out]

 The <b>BSTR</b> representation of the terminal's 
<a href="https://msdn.microsoft.com/2a16d33c-2d87-4172-a5ff-33ff62e96615">terminal class</a>. The <b>BSTR</b> is allocated using 
<a href="https://msdn.microsoft.com/en-us/library/ms221458(v=VS.85).aspx">SysAllocString</a>. It should be deallocated by the client.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/0f7190c4-c696-4749-82f2-20fdbc8651f4">ITPluggableTerminalClassInfo</a>
 

 

