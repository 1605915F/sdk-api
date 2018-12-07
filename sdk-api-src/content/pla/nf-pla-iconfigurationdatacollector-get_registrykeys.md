---
UID: NF:pla.IConfigurationDataCollector.get_RegistryKeys
title: IConfigurationDataCollector::get_RegistryKeys
author: windows-sdk-content
description: Retrieves or sets a list of registry keys to collect.
old-location: pla\iconfigurationdatacollector_registrykeys.htm
tech.root: pla
ms.assetid: 990a5f92-2285-4461-8020-25028d2cab90
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: IConfigurationDataCollector interface [PLA],RegistryKeys property, IConfigurationDataCollector.RegistryKeys, IConfigurationDataCollector.get_RegistryKeys, IConfigurationDataCollector::RegistryKeys, IConfigurationDataCollector::get_RegistryKeys, IConfigurationDataCollector::put_RegistryKeys, RegistryKeys property [PLA], RegistryKeys property [PLA],IConfigurationDataCollector interface, base.iconfigurationdatacollector_registrykeys, get_RegistryKeys, pla.iconfigurationdatacollector_registrykeys, pla/IConfigurationDataCollector::RegistryKeys, pla/IConfigurationDataCollector::get_RegistryKeys, pla/IConfigurationDataCollector::put_RegistryKeys
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: pla.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: Pla.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Pla.dll
api_name:
 - IConfigurationDataCollector.RegistryKeys
 - IConfigurationDataCollector.get_RegistryKeys
 - IConfigurationDataCollector.put_RegistryKeys
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IConfigurationDataCollector::get_RegistryKeys


## -description


Retrieves or sets a list of registry keys to collect.

This property is read/write.


## -parameters


## -remarks



You can collect registry data from the following registry hives:

<ul>
<li><b>HKEY_CLASSES_ROOT</b></li>
<li><b>HKEY_CURRENT_CONFIG</b></li>
<li><b>HKEY_CURRENT_USER</b></li>
<li><b>HKEY_LOCAL_MACHINE</b></li>
<li><b>HKEY_USERS</b></li>
</ul>
To collect a registry value, specify the full path to the value name, for example, <b>\HKEY_LOCAL_MACHINE\MyKey\MyValue</b>.

To collect all the values under a registry key, specify the full path to the registry key, for example, <b>\HKEY_LOCAL_MACHINE\MyKey\</b>.

To collect all the values under a registry key and its subkeys, use two backslashes for the last path delimiter, for example, <b>\\computername\HKEY_LOCAL_MACHINE\MyKey\\</b>. PLA recursively collects the registry data down to the level specified in the <a href="https://msdn.microsoft.com/f291a404-a952-42cd-a538-c7d326aa29d8">IConfigurationDataCollector::RegistryMaxRecursiveDepth</a> property.

To collect registry information from a remote computer, include the computer name at the beginning of the registry path, for example, <b>\\computername\HKEY_LOCAL_MACHINE\MyKey\MyValue</b>.




## -see-also




<a href="https://msdn.microsoft.com/7266c02d-0f56-4754-8a67-68394a5f0158">IConfigurationDataCollector</a>



<a href="https://msdn.microsoft.com/f291a404-a952-42cd-a538-c7d326aa29d8">IConfigurationDataCollector::RegistryMaxRecursiveDepth</a>
 

 

