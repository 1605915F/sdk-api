---
UID: NF:mswmdm.IMDSPRevoked.GetRevocationURL
title: IMDSPRevoked::GetRevocationURL (mswmdm.h)
author: windows-sdk-content
description: The GetRevocationURL method retrieves the URL from which updated components can be downloaded.
old-location: wmdm\imdsprevoked_getrevocationurl.htm
tech.root: WMDM
ms.assetid: 414eddd0-be05-4f23-ae94-2c6210220729
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetRevocationURL, GetRevocationURL method [windows Media Device Manager], GetRevocationURL method [windows Media Device Manager],IMDSPRevoked interface, IMDSPRevoked interface [windows Media Device Manager],GetRevocationURL method, IMDSPRevoked.GetRevocationURL, IMDSPRevoked::GetRevocationURL, IMDSPRevokedGetRevocationURL, mswmdm/IMDSPRevoked::GetRevocationURL, wmdm.imdsprevoked_getrevocationurl
ms.topic: method
req.header: mswmdm.h
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
req.lib: Mssachlp.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mssachlp.lib
 - mssachlp.dll
api_name:
 - IMDSPRevoked.GetRevocationURL
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMDSPRevoked::GetRevocationURL


## -description



The <b>GetRevocationURL</b> method retrieves the URL from which updated components can be downloaded.




## -parameters




### -param ppwszRevocationURL [in, out]

Pointer to a Unicode string where the revocation URL should be written.


### -param pdwBufferLen [in, out]

Number of <b>WCHAR</b> characters that the buffer supplied by the client can hold; on return it contains the required number of characters.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -remarks



The <b>IMDSPRevoked</b> interface retrieves the URL from which updated components can be downloaded if the service provider is ever revoked by any digital rights management system. If this method is not implemented, a default Microsoft URL will be used. This location is maintained by Microsoft and contains updates to components revoked by the Microsoft digital rights management system.




## -see-also




<a href="https://msdn.microsoft.com/8df545b9-52f5-422e-a0c1-2316c628d89f">IMDSPRevoked Interface</a>
 

 

