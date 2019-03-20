---
UID: NE:inspectable.TrustLevel
title: TrustLevel (inspectable.h)
author: windows-sdk-content
description: Represents the trust level of an activatable class.
old-location: winrt\trustlevel.htm
tech.root: WinRT
ms.assetid: 75E30E4B-EE5F-41C4-AC22-91D542E920EB
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BaseTrust, FullTrust, PartialTrust, RegisteredTrustLevel, TrustLevel, TrustLevel enumeration [Windows Runtime], inspectable/BaseTrust, inspectable/FullTrust, inspectable/PartialTrust, inspectable/TrustLevel, winrt.trustlevel
ms.topic: enum
req.header: inspectable.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Inspectable.idl
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
 - Inspectable.h
api_name:
 - TrustLevel
product: Windows
targetos: Windows
req.typenames: TrustLevel
req.redist: 
---

# TrustLevel enumeration


## -description


Represents the trust level of an activatable class.


## -enum-fields




### -field BaseTrust

The component has access to resources that are not protected.


### -field PartialTrust

The component has access to resources requested in the app manifest and approved by the user.


### -field FullTrust

The component requires the full privileges of the user.


## -remarks



Classes can be activated depending on the trust level of the caller and the trust classification of the activatable class.


<a href="https://msdn.microsoft.com/1B579206-F6B9-47C1-A7F3-4E7ECDEDCBB4">RegisteredTrustLevel</a> is an alias for this enumeration. 




## -see-also




<a href="https://msdn.microsoft.com/E7E8AFD1-A8B7-4023-9F8B-573E0D2622F6">IInspectable::GetTrustLevel</a>
 

 

