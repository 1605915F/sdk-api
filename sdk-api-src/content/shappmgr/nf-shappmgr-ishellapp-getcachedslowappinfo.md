---
UID: NF:shappmgr.IShellApp.GetCachedSlowAppInfo
title: IShellApp::GetCachedSlowAppInfo (shappmgr.h)
author: windows-sdk-content
description: Returns information to the application that originates from a slow source. Unlike IShellApp::GetSlowAppInfo, this method can return information that has been cached. This method is not applicable to published applications.
old-location: shell\IShellApp_GetCachedSlowAppInfo.htm
tech.root: shell
ms.assetid: 655edc51-0967-4b94-9eef-da213e735e0a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCachedSlowAppInfo, GetCachedSlowAppInfo method [Windows Shell], GetCachedSlowAppInfo method [Windows Shell],IShellApp interface, IShellApp interface [Windows Shell],GetCachedSlowAppInfo method, IShellApp.GetCachedSlowAppInfo, IShellApp::GetCachedSlowAppInfo, inet_IShellApp_GetCachedSlowAppInfo, shappmgr/IShellApp::GetCachedSlowAppInfo, shell.IShellApp_GetCachedSlowAppInfo
ms.topic: method
req.header: shappmgr.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shappmgr.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Shell32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Shell32.dll
api_name:
 - IShellApp.GetCachedSlowAppInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IShellApp::GetCachedSlowAppInfo


## -description


Returns information to the application that originates from a slow source. Unlike <a href="https://msdn.microsoft.com/02f8e527-1c3c-4a2e-bf55-4f33c6a7b822">IShellApp::GetSlowAppInfo</a>, this method can return information that has been cached. This method is not applicable to published applications.


## -parameters




### -param psaid [out]

Type: <b>PSLOWAPPINFO</b>

A pointer to a <a href="https://msdn.microsoft.com/e9af8c70-0f03-4f16-bbfb-5e54f7c6c9df">SLOWAPPINFO</a> structure in which to return application information.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Implementations of <a href="https://msdn.microsoft.com/a5a44e74-494a-4c9b-8bf3-85c6093b2c0e">IPublishedApp</a> return E_NOTIMPL. This method is used internally by Add/Remove Programs for installed applications.




## -see-also




<a href="https://msdn.microsoft.com/5391444a-53b6-48c9-9a94-d045b3f97182">IAppPublisher</a>



<a href="https://msdn.microsoft.com/a5a44e74-494a-4c9b-8bf3-85c6093b2c0e">IPublishedApp</a>



<a href="https://msdn.microsoft.com/2f56744c-a10e-423f-8b8f-c3257e560310">IShellApp</a>
 

 

