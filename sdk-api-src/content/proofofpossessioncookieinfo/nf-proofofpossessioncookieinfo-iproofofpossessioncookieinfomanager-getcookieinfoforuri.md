---
UID: NF:proofofpossessioncookieinfo.IProofOfPossessionCookieInfoManager.GetCookieInfoForUri
title: IProofOfPossessionCookieInfoManager::GetCookieInfoForUri
author: windows-sdk-content
description: Gets cookie information for the supplied URI to be used for proof of possession cookies.
old-location: wininet\iproofofpossessioncookieinfomanager_getcookieinfoforuri.htm
tech.root: wininet
ms.assetid: e7e22e0e-f84c-47e5-878f-b70459c921b8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCookieInfoForUri, GetCookieInfoForUri method [WinINet], GetCookieInfoForUri method [WinINet],IProofOfPossessionCookieInfoManager interface, IProofOfPossessionCookieInfoManager interface [WinINet],GetCookieInfoForUri method, IProofOfPossessionCookieInfoManager.GetCookieInfoForUri, IProofOfPossessionCookieInfoManager::GetCookieInfoForUri, proofofpossessioncookieinfo/IProofOfPossessionCookieInfoManager::GetCookieInfoForUri, wininet.iproofofpossessioncookieinfomanager_getcookieinfoforuri
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: proofofpossessioncookieinfo.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ProofOfPossessionCookieInfo.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: MicrosoftAccountTokenProvider.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - MicrosoftAccountTokenProvider.dll
api_name:
 - IProofOfPossessionCookieInfoManager.GetCookieInfoForUri
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IProofOfPossessionCookieInfoManager::GetCookieInfoForUri


## -description


Gets cookie information for the supplied URI to be used for proof of possession cookies.


## -parameters




### -param uri [in]

The URI to get cookie information for. The URI is case-sensitive.


### -param cookieInfoCount [out]

The number of cookies found for the <i>uri</i>.


### -param cookieInfo [out]

The cookie information for the <i>uri</i>.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/b8b89e48-e47d-4089-a8b6-04d53227767a">IProofOfPossessionCookieInfoManager</a>
 

 

