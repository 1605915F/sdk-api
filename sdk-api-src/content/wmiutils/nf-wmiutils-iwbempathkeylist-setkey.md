---
UID: NF:wmiutils.IWbemPathKeyList.SetKey
title: IWbemPathKeyList::SetKey
author: windows-sdk-content
description: Sets the name or value pair for a key.
old-location: wmi\iwbempathkeylist_setkey.htm
tech.root: WmiSdk
ms.assetid: d655c5c7-0830-46fc-a81d-9bfa16f80d68
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWbemPathKeyList interface [Windows Management Instrumentation],SetKey method, IWbemPathKeyList.SetKey, IWbemPathKeyList::SetKey, SetKey, SetKey method [Windows Management Instrumentation], SetKey method [Windows Management Instrumentation],IWbemPathKeyList interface, _hmm_iwbempathkeylist_setkey, wmi.iwbempathkeylist_setkey, wmiutils/IWbemPathKeyList::SetKey
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IWbemPathKeyList.SetKey
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWbemPathKeyList::SetKey


## -description


The 
<b>IWbemPathKeyList::SetKey</b> method sets the name or value pair for a key. If the key exists, it is replaced. If the name is empty, all existing keys are deleted.


## -parameters




### -param wszName [in]

Key name, may be <b>NULL</b>.


### -param uFlags [in]

Reserved. Must be 0 (zero).


### -param uCimType [in]

CIMTYPE size.


### -param pKeyVal [in]

Pointer to the data. The data pointed to varies depending on the <i>uCimType</i> parameter.


## -returns



This method returns an <b>HRESULT</b> indicating the status of the method call.




## -see-also




<a href="https://msdn.microsoft.com/71b2597b-d82a-439d-b0b7-af76aefea6a2">IWbemPath</a>



<a href="https://msdn.microsoft.com/5b188426-9d7f-4e87-9eed-ce80e5d93c30">IWbemPathKeyList</a>



<a href="https://msdn.microsoft.com/3b282124-d544-405a-96e0-39cc504c8117">IWbemPathKeyList::SetKey2</a>
 

 

