---
UID: NF:wtsprotocol.IWRdsProtocolConnection.AcceptConnection
title: IWRdsProtocolConnection::AcceptConnection
author: windows-sdk-content
description: Directs the protocol to continue with the connection request.
old-location: termserv\iwrdsprotocolconnection_acceptconnection.htm
tech.root: TermServ
ms.assetid: ef7e13ad-eeb8-4452-b3d6-a137b766f98f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AcceptConnection, AcceptConnection method [Remote Desktop Services], AcceptConnection method [Remote Desktop Services],IWRdsProtocolConnection interface, IWRdsProtocolConnection interface [Remote Desktop Services],AcceptConnection method, IWRdsProtocolConnection.AcceptConnection, IWRdsProtocolConnection::AcceptConnection, termserv.iwrdsprotocolconnection_acceptconnection, wtsprotocol/IWRdsProtocolConnection::AcceptConnection
ms.topic: method
req.header: wtsprotocol.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wtsprotocol.idl
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
 - COM
api_location:
 - wtsprotocol.h
api_name:
 - IWRdsProtocolConnection.AcceptConnection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWRdsProtocolConnection::AcceptConnection


## -description


Directs the protocol to continue with the connection request.


## -parameters






## -returns



If this method succeeds, it returns <b>S_OK</b>. Otherwise, it returns an <b>HRESULT</b> error code.

Upon receiving an error, the Remote Desktop Services service will drop the connection.




## -see-also




<a href="https://msdn.microsoft.com/2b8a5b2f-5a54-4d60-8b5a-8a914728087c">IWRdsProtocolConnection</a>
 

 

