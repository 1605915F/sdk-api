---
UID: NF:wmiutils.IWbemPath.IsRelativeOrChild
title: IWbemPath::IsRelativeOrChild (wmiutils.h)
author: windows-sdk-content
description: The IWbemPath::IsRelativeOrChild method tests if the path, as already set in the parser, is relative to or a child of a particular computer and namespace.
old-location: wmi\iwbempath_isrelativeorchild.htm
tech.root: WmiSdk
ms.assetid: 95ba21af-3a43-4aa9-ab5b-90712e9cbed1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWbemPath interface [Windows Management Instrumentation],IsRelativeOrChild method, IWbemPath.IsRelativeOrChild, IWbemPath::IsRelativeOrChild, IsRelativeOrChild, IsRelativeOrChild method [Windows Management Instrumentation], IsRelativeOrChild method [Windows Management Instrumentation],IWbemPath interface, _hmm_iwbempath_isrelativeorchild, wmi.iwbempath_isrelativeorchild, wmiutils/IWbemPath::IsRelativeOrChild
ms.topic: method
req.header: wmiutils.h
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
req.lib: Wbemuuid.lib
req.dll: Wmiutils.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wmiutils.dll
api_name:
 - IWbemPath.IsRelativeOrChild
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWbemPath::IsRelativeOrChild


## -description


The 
<b>IWbemPath::IsRelativeOrChild</b> method tests if the path, as already set in the parser, is relative to or a child of a particular computer and namespace.


## -parameters




### -param wszMachine [in]

Name of the computer.


### -param wszNamespace [in]

Namespace being tested.


### -param lFlags [in]

Reserved. Must be 0 (zero).


## -returns



This method returns a <b>BOOL</b> indicating whether the path is relative to the specified computer and namespace.




## -see-also




<a href="https://msdn.microsoft.com/71b2597b-d82a-439d-b0b7-af76aefea6a2">IWbemPath</a>



<a href="https://msdn.microsoft.com/5b188426-9d7f-4e87-9eed-ce80e5d93c30">IWbemPathKeyList</a>
 

 

