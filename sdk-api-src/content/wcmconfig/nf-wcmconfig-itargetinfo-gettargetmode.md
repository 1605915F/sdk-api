---
UID: NF:wcmconfig.ITargetInfo.GetTargetMode
title: ITargetInfo::GetTargetMode
author: windows-sdk-content
description: Gets the current target mode.
old-location: smi\itargetinfo_gettargetmode.htm
tech.root: SMI
ms.assetid: b21137a0-537f-43a4-857b-158a1642ea1c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetTargetMode, GetTargetMode method [SMI], GetTargetMode method [SMI],ITargetInfo interface, ITargetInfo interface [SMI],GetTargetMode method, ITargetInfo.GetTargetMode, ITargetInfo::GetTargetMode, smi.itargetinfo_gettargetmode, wcmconfig/ITargetInfo::GetTargetMode
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wcmconfig.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WcmConfig.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: SMIEngine.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - SMIEngine.dll
api_name:
 - ITargetInfo.GetTargetMode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITargetInfo::GetTargetMode


## -description


Gets the current target mode.


## -parameters




### -param TargetMode [out]

The current target mode. The target mode identifies the way in which the redirections from the target are handled.


## -returns



This method returns an HRESULT value. <b>S_OK</b> indicates success.




## -see-also




<a href="https://msdn.microsoft.com/f1dd3c93-43ca-4804-8330-55acaccf8ea8">ITargetInfo</a>
 

 

