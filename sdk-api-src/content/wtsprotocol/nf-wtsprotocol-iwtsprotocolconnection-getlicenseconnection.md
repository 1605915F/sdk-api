---
UID: NF:wtsprotocol.IWTSProtocolConnection.GetLicenseConnection
title: IWTSProtocolConnection::GetLicenseConnection (wtsprotocol.h)
author: windows-sdk-content
description: IWTSProtocolConnection::GetLicenseConnection is no longer available. Instead, use IWRdsProtocolConnection::GetLicenseConnection.
old-location: termserv\iwtsprotocolconnection_getlicenseconnection.htm
tech.root: TermServ
ms.assetid: 714e2479-54b2-4899-9fbd-68fa35051f58
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetLicenseConnection, GetLicenseConnection method [Remote Desktop Services], GetLicenseConnection method [Remote Desktop Services],IWTSProtocolConnection interface, IWTSProtocolConnection interface [Remote Desktop Services],GetLicenseConnection method, IWTSProtocolConnection.GetLicenseConnection, IWTSProtocolConnection::GetLicenseConnection, termserv.iwtsprotocolconnection_getlicenseconnection, wtsprotocol/IWTSProtocolConnection::GetLicenseConnection
ms.topic: method
req.header: wtsprotocol.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2
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
 - Wtsprotocol.h
api_name:
 - IWTSProtocolConnection.GetLicenseConnection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWTSProtocolConnection::GetLicenseConnection


## -description


<p class="CCE_Message">[<b>IWTSProtocolConnection::GetLicenseConnection</b> is no longer available for use as of Windows Server 2012. Instead, use <a href="https://msdn.microsoft.com/6c75f80a-0d47-489d-b684-f718326e2b0d">IWRdsProtocolConnection::GetLicenseConnection</a>.]

Retrieves an <a href="https://msdn.microsoft.com/3f6925b6-c712-40c6-8b48-7df8ef4a9872">IWTSProtocolLicenseConnection</a> object that is used to begin the client licensing process. The protocol must add a reference to this object before returning. When the Remote Desktop Services service has finished the licensing process, it will release the reference.


## -parameters




### -param ppLicenseConnection [out]

The address of a pointer to an <a href="https://msdn.microsoft.com/3f6925b6-c712-40c6-8b48-7df8ef4a9872">IWTSProtocolLicenseConnection</a> interface.


## -see-also




<a href="https://msdn.microsoft.com/584a6874-0df4-480e-a10a-4b603643870e">IWTSProtocolConnection</a>
 

 

