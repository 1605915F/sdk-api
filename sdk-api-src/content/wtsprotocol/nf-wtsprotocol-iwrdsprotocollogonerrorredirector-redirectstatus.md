---
UID: NF:wtsprotocol.IWRdsProtocolLogonErrorRedirector.RedirectStatus
title: IWRdsProtocolLogonErrorRedirector::RedirectStatus
author: windows-sdk-content
description: Queries the protocol regarding how to redirect the client logon status update.
old-location: termserv\iwrdsprotocollogonerrorredirector_redirectstatus.htm
tech.root: termserv
ms.assetid: f1f6caec-6e26-4508-b19d-ac0e12758b28
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWRdsProtocolLogonErrorRedirector interface [Remote Desktop Services],RedirectStatus method, IWRdsProtocolLogonErrorRedirector.RedirectStatus, IWRdsProtocolLogonErrorRedirector::RedirectStatus, RedirectStatus, RedirectStatus method [Remote Desktop Services], RedirectStatus method [Remote Desktop Services],IWRdsProtocolLogonErrorRedirector interface, termserv.iwrdsprotocollogonerrorredirector_redirectstatus, wtsprotocol/IWRdsProtocolLogonErrorRedirector::RedirectStatus
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
 - IWRdsProtocolLogonErrorRedirector.RedirectStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWRdsProtocolLogonErrorRedirector::RedirectStatus


## -description


Queries the protocol regarding how to redirect the client logon status update.


## -parameters




### -param pszMessage [in]

A pointer to a string that contains the logon status message.


### -param pResponse [out]

A pointer to a <a href="https://msdn.microsoft.com/67ed8d6f-641c-4739-911c-e61379e14048">WRDS_LOGON_ERROR_REDIRECTOR_RESPONSE</a> enumeration that contains the response.


## -returns



When you are implementing this method, return <b>S_OK</b> if the function succeeds. If it fails, return an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>. 




## -see-also




<a href="https://msdn.microsoft.com/43c283f5-c902-49cc-81a0-15fc6316c7d4">IWRdsProtocolLogonErrorRedirector</a>
 

 

