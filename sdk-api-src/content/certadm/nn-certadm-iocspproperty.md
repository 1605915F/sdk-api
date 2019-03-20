---
UID: NN:certadm.IOCSPProperty
title: IOCSPProperty (certadm.h)
author: windows-sdk-content
description: Represents a name-value pair for OCSPServiceProperties or ProviderProperties.
old-location: security\iocspproperty.htm
tech.root: SecCrypto
ms.assetid: 854848f0-ea89-4c25-a8a5-40f1e4d229be
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOCSPProperty, IOCSPProperty interface [Security], IOCSPProperty interface [Security],described, certadm/IOCSPProperty, security.iocspproperty
ms.topic: interface
req.header: certadm.h
req.include-header: Certserv.h
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Datacenter, Windows Server 2008 Enterprise [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certadm.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Certadm.lib
req.dll: Certadm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certadm.dll
api_name:
 - IOCSPProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCSPProperty interface


## -description


The <b>IOCSPProperty</b> interface represents a name-value pair for <a href="https://msdn.microsoft.com/d792283b-dde9-46b7-8483-b3011b4433eb">OCSPServiceProperties</a> or <a href="https://msdn.microsoft.com/60ac0123-9696-4893-ae2a-278b4e70c098">ProviderProperties</a>.

Microsoft provides a default implementation of this interface in the <b>OCSPProperty</b> class. An <b>OCSPProperty</b> object cannot be created externally.

The default implementation of <a href="https://msdn.microsoft.com/8c700357-0cb4-4780-9ff1-ac57c46f9183">IOCSPPropertyCollection</a> methods creates an <b>OCSPProperty</b> object and uses its properties.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>
 

 

