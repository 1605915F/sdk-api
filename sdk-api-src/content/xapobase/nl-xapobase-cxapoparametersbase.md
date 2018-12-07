---
UID: NL:xapobase.CXAPOParametersBase
title: CXAPOParametersBase
author: windows-sdk-content
description: Default implementation of the IXAPOParameters interface.
old-location: xaudio2\cxapoparametersbase.htm
tech.root: xaudio2
ms.assetid: T:Microsoft.directx_sdk.cxapoparameterbase.CXAPOParametersBase
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CXAPOParametersBase, CXAPOParametersBase class [XAudio2 Audio Mixing APIs], CXAPOParametersBase class [XAudio2 Audio Mixing APIs],described, xapobase/CXAPOParametersBase, xaudio2.cxapoparametersbase
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: class
req.header: xapobase.h
req.include-header: 
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
req.lib: XAPOBase.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - XAPOBase.lib
 - XAPOBase.dll
api_name:
 - CXAPOParametersBase
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CXAPOParametersBase class


## -description


Default implementation of the <a href="https://msdn.microsoft.com/en-us/library/Ee415896(v=VS.85).aspx">IXAPOParameters</a> interface.

For a list of all members of this class, see <a href="https://msdn.microsoft.com/en-us/library/Ee415239(v=VS.85).aspx">CXAPOParametersBase Members</a>.


## -remarks



<b>CXAPOParametersBase</b> provides thread-safe, overridable implementations for all <a href="https://msdn.microsoft.com/en-us/library/Ee415896(v=VS.85).aspx">IXAPOParameters</a> methods.



This class is for parameter blocks whose size is larger than 8 bytes. To achieve synchronization of smaller parameter blocks, use Interlocked operations directly on the parameters.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Windows 10 (XAudio2.9); Windows 8, Windows Phone 8 (XAudio 2.8); DirectX SDK (XAudio 2.7)




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ee415236(v=VS.85).aspx">CXAPOBase</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415239(v=VS.85).aspx">CXAPOParametersBase Members</a>



<a href="https://msdn.microsoft.com/4349f03a-54a0-2780-0138-a893e1568a26">Classes</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415896(v=VS.85).aspx">IXAPOParameters</a>
 

 

