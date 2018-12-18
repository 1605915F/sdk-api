---
UID: NF:wsmandisp.IWSManSession.Create
title: IWSManSession::Create
author: windows-sdk-content
description: Creates a new instance of a resource and returns the endpoint reference (EPR) of the new object.
old-location: winrm\iwsmansession_create.htm
tech.root: winrm
ms.assetid: 7e8b561e-c724-427b-88a0-34a6c8a9c6bd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Create, Create method [Windows Remote Management], Create method [Windows Remote Management],IWSManSession interface, IWSManSession interface [Windows Remote Management],Create method, IWSManSession.Create, IWSManSession::Create, winrm.iwsmansession_create, wsmandisp/IWSManSession::Create
ms.topic: method
req.header: wsmandisp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WSManDisp.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WSManDisp.tlb
req.dll: WSMAuto.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - WSMAuto.dll
api_name:
 - IWSManSession.Create
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWSManSession::Create


## -description


Creates a new instance of a resource and returns the <a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">endpoint reference</a> (EPR) of the new object.


## -parameters




### -param resourceUri [in]

The identifier of the resource to create.

This parameter can contain one of the following:

<ul>
<li>URI with one or more  <a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">selectors</a>. Be aware that the <a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">WMI plug-in</a> does not support creating any resource other than a WS-Management protocol listener.</li>
<li>
<a href="https://msdn.microsoft.com/0904b7eb-d4ce-46a7-bf58-452e7c0d41e9">ResourceLocator</a> object which may contain selectors,  <a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">fragments</a>, or <a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">options</a>.</li>
<li><a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">WS-Addressing</a> endpoint reference as described in the WS-Management protocol  standard.  For more information about the public specification for the WS-Management protocol, see  <a href="http://go.microsoft.com/fwlink/p/?linkid=84316">Management Specifications Index Page</a>.</li>
</ul>

### -param resource [in]

An XML string that contains resource content.


### -param flags [in]

Reserved. Must be set to 0.


### -param newUri [out]

The EPR of the new resource.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<b>IWSManSession::Create</b> is only used for creating new 
    instances of a resource. Use the <a href="https://msdn.microsoft.com/1224dab8-82d1-4416-8c21-e84fdda15deb">IWSManSession::Put</a> method to 
    update existing instances of a resource. After you obtain the new resource URI, you can call 
    <a href="https://msdn.microsoft.com/f6393cfb-0787-4d30-8d02-be0996885f22">IWSManSession::Get</a> to retrieve the new object. The new object 
    contains any properties that the resource provider assigns when creating the new object. For example, if you 
    create a new WS-Management protocol<a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">listener</a> and retrieve the listener object using <a href="https://msdn.microsoft.com/873242fd-9da3-42f4-a18e-258fedba77ec">Session.Get</a>, then you also obtain the <b>Port</b>, <b>Enabled</b>, and <b>ListeningOn</b> properties.




## -see-also




<a href="https://msdn.microsoft.com/3e016080-339f-4bda-bfd2-f912e090981f">IWSManSession</a>



<a href="https://msdn.microsoft.com/7629dfff-6c66-4b09-81a4-b1458ff977fa">Session.Create</a>
 

 

