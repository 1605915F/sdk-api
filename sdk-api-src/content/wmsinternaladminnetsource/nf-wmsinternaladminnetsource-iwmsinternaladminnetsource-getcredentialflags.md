---
UID: NF:wmsinternaladminnetsource.IWMSInternalAdminNetSource.GetCredentialFlags
title: IWMSInternalAdminNetSource::GetCredentialFlags (wmsinternaladminnetsource.h)
author: windows-sdk-content
description: The GetCredentialFlags method can be used in conjunction with IWMSInternalAdminNetSource::SetCredentialFlags to determine whether the user wants passwords saved as a default behavior. This method retrieves any flags previously set.
old-location: wmformat\iwmsinternaladminnetsource_getcredentialflags.htm
tech.root: wmformat
ms.assetid: 781b2868-c8e2-4d92-98f2-c2950fac3d9b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCredentialFlags, GetCredentialFlags method [windows Media Format], GetCredentialFlags method [windows Media Format],IWMSInternalAdminNetSource interface, IWMSInternalAdminNetSource interface [windows Media Format],GetCredentialFlags method, IWMSInternalAdminNetSource.GetCredentialFlags, IWMSInternalAdminNetSource::GetCredentialFlags, IWMSInternalAdminNetSourceGetCredentialFlags, wmformat.iwmsinternaladminnetsource_getcredentialflags, wmsinternaladminnetsource/IWMSInternalAdminNetSource::GetCredentialFlags
ms.topic: method
req.header: wmsinternaladminnetsource.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wmvcore.lib
 - Wmvcore.dll
 - WMStubDRM.lib
 - WMStubDRM.dll
api_name:
 - IWMSInternalAdminNetSource.GetCredentialFlags
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMSInternalAdminNetSource::GetCredentialFlags


## -description



The <b>GetCredentialFlags</b> method can be used in conjunction with <a href="https://msdn.microsoft.com/en-us/library/Dd798541(v=VS.85).aspx">IWMSInternalAdminNetSource::SetCredentialFlags</a> to determine whether the user wants passwords saved as a default behavior. This method retrieves any flags previously set.




## -parameters




### -param lpdwFlags [out]

<b>DWORD</b> containing credential flags. At this time, the only supported flag is 0x1, which signifies that the user has stated a preference that passwords should be saved automatically.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd743717(v=VS.85).aspx">IWMSInternalAdminNetSource Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798539(v=VS.85).aspx">IWMSInternalAdminNetSource::GetCredentials</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd798541(v=VS.85).aspx">IWMSInternalAdminNetSource::SetCredentialFlags</a>
 

 

