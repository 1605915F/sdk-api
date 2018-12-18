---
UID: NF:wsmandisp.IWSManResourceLocator.AddSelector
title: IWSManResourceLocator::AddSelector
author: windows-sdk-content
description: Adds a selector to the ResourceLocator object. The selector specifies a particular instance of a resource.
old-location: winrm\iwsmanresourcelocator_addselector.htm
tech.root: winrm
ms.assetid: 2f6c1169-8e2a-4919-9a1a-856dbe41a9ce
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddSelector, AddSelector method [Windows Remote Management], AddSelector method [Windows Remote Management],IWSManResourceLocator interface, IWSManResourceLocator interface [Windows Remote Management],AddSelector method, IWSManResourceLocator.AddSelector, IWSManResourceLocator::AddSelector, winrm.iwsmanresourcelocator_addselector, wsmandisp/IWSManResourceLocator::AddSelector
ms.topic: method
req.header: wsmandisp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WSManDisp.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WSManDisp.tlb
req.dll: WSMAuto.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - WSMAuto.dll
api_name:
 - IWSManResourceLocator.AddSelector
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWSManResourceLocator::AddSelector


## -description


Adds a <a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">selector</a> to the <a href="https://msdn.microsoft.com/0904b7eb-d4ce-46a7-bf58-452e7c0d41e9">ResourceLocator</a> object. The selector specifies a particular instance of a <i>resource</i>. You can provide an <a href="https://msdn.microsoft.com/7b3dcb53-d02c-4ba6-973d-1493ba442387">IWSManResourceLocator</a> object instead of specifying a resource URI in <a href="https://msdn.microsoft.com/3e016080-339f-4bda-bfd2-f912e090981f">IWSManSession</a> object operations such as <a href="https://msdn.microsoft.com/f6393cfb-0787-4d30-8d02-be0996885f22">Get</a>, <a href="https://msdn.microsoft.com/1224dab8-82d1-4416-8c21-e84fdda15deb">Put</a>, or <a href="https://msdn.microsoft.com/b1a4815e-93aa-4a30-a67e-c52fd06c1ee1">Enumerate</a>.


## -parameters




### -param resourceSelName [in]

The selector name. For example, when requesting WMI data, this parameter is the key property for a WMI class.


### -param selValue [in]

The selector value. For example, for WMI data, this parameter contains a value for a key property that identifies a specific instance.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/7b3dcb53-d02c-4ba6-973d-1493ba442387">IWSManResourceLocator</a>



<a href="https://msdn.microsoft.com/4b513d39-a377-487f-a03b-f3c5ab0f0b5a">ResourceLocator.AddSelector</a>
 

 

