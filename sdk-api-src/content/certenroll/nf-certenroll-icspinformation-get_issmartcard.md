---
UID: NF:certenroll.ICspInformation.get_IsSmartCard
title: ICspInformation::get_IsSmartCard
author: windows-sdk-content
description: Retrieves a Boolean value that specifies whether the provider is a smart card provider.
old-location: security\icspinformation_issmartcard_property.htm
tech.root: seccertenroll
ms.assetid: cfb88e17-39bb-4b4f-9eb3-3691376f8285
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICspInformation interface [Security],IsSmartCard property, ICspInformation.IsSmartCard, ICspInformation.get_IsSmartCard, ICspInformation::IsSmartCard, ICspInformation::get_IsSmartCard, IsSmartCard property [Security], IsSmartCard property [Security],ICspInformation interface, certenroll/ICspInformation::IsSmartCard, certenroll/ICspInformation::get_IsSmartCard, get_IsSmartCard, security.icspinformation_issmartcard_property
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenroll.h
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
req.dll: CertEnroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CertEnroll.dll
api_name:
 - ICspInformation.IsSmartCard
 - ICspInformation.get_IsSmartCard
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICspInformation::get_IsSmartCard


## -description


The <b>IsSmartCard</b> property retrieves a Boolean value that specifies whether the provider is a smart card provider.

This property is read-only.


## -parameters


## -remarks



A smart card provider is typically identified by the <a href="https://msdn.microsoft.com/en-us/library/Aa376747(v=VS.85).aspx">IsHardwareDevice</a> property and the <a href="https://msdn.microsoft.com/en-us/library/Aa376750(v=VS.85).aspx">IsSoftwareDevice</a> property being set or the <a href="https://msdn.microsoft.com/en-us/library/Aa376748(v=VS.85).aspx">IsRemovable</a> property being set.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa375967(v=VS.85).aspx">ICspInformation</a>
 

 

