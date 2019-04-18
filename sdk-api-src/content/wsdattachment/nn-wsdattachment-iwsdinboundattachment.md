---
UID: NN:wsdattachment.IWSDInboundAttachment
title: IWSDInboundAttachment (wsdattachment.h)
author: windows-sdk-content
description: Allows applications to read MIME-encoded attachment data from an incoming message.
old-location: ncd\iwsdinboundattachment.htm
tech.root: WsdApi
ms.assetid: 1bacbf20-2eb2-4aa1-ba37-e14dc0d955b0
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWSDInboundAttachment, IWSDInboundAttachment interface, IWSDInboundAttachment interface,described, ncd.iwsdinboundattachment, wsdattachment/IWSDInboundAttachment
ms.topic: interface
req.header: wsdattachment.h
req.include-header: Wsdapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WsdAttachment.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Wsdapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wsdapi.dll
api_name:
 - IWSDInboundAttachment
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWSDInboundAttachment interface


## -description


Allows applications to read MIME-encoded attachment data from an incoming message.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWSDInboundAttachment</b> interface inherits from <a href="https://msdn.microsoft.com/9acbbca2-9b43-4bed-8917-be99f13fce13">IWSDAttachment</a>. <b>IWSDInboundAttachment</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWSDInboundAttachment</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1bd0295c-4c37-42ec-b5a5-dc7f467def05">Close</a>
</td>
<td align="left" width="63%">
Closes the current attachment MIME data stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/66b8ce84-23b3-43f2-826d-c866b8bedab1">Read</a>
</td>
<td align="left" width="63%">
Reads attachment data from a message sent by a remote host.

</td>
</tr>
</table> 


## -remarks



WSDAPI will provide an object implementing this interface when an attachment stream is received as part of a message.




## -see-also




<a href="https://msdn.microsoft.com/9acbbca2-9b43-4bed-8917-be99f13fce13">IWSDAttachment</a>
 

 

