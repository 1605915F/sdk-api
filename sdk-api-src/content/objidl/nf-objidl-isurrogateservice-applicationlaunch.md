---
UID: NF:objidl.ISurrogateService.ApplicationLaunch
title: ISurrogateService::ApplicationLaunch (objidl.h)
author: windows-sdk-content
description: Launches the application.
old-location: com\isurrogateservice_applicationlaunch.htm
tech.root: com
ms.assetid: 4e54c129-f321-4215-b084-21ab17f93a6f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ApplicationLaunch, ApplicationLaunch method [COM], ApplicationLaunch method [COM],ISurrogateService interface, ISurrogateService interface [COM],ApplicationLaunch method, ISurrogateService.ApplicationLaunch, ISurrogateService::ApplicationLaunch, _com_isurrogateservice_applicationlaunch, com.isurrogateservice_applicationlaunch, objidl/ISurrogateService::ApplicationLaunch
ms.topic: method
req.header: objidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ObjIdl.idl
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
 - ObjIdl.h
api_name:
 - ISurrogateService.ApplicationLaunch
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISurrogateService::ApplicationLaunch


## -description


Launches the application.


## -parameters




### -param rguidApplID [in]

The application identifier.


### -param appType [in]

The application type, as described in Remarks.


## -returns



If the method succeeds, the return value is S_OK. Otherwise, it is E_UNEXPECTED.




## -remarks



The application type is defined by the following enum.

<pre class="syntax" xml:space="preserve"><code>typedef enum tagApplicationType { 
    ServerApplication, 
    LibraryApplication 
} ApplicationType;
</code></pre>



## -see-also




<a href="https://msdn.microsoft.com/d1ffee1d-f907-4091-b993-cf13d8ce616c">CoGetInterceptor</a>



<a href="https://msdn.microsoft.com/56a75123-f402-4187-af13-d31f72a5f094">ICallFrame</a>



<a href="https://msdn.microsoft.com/2f1e1b8d-6150-45e9-89e2-524d80df558d">ICallFrameEvents</a>



<a href="https://msdn.microsoft.com/d0a72c87-598b-4ebe-bc93-65e0927a4c3d">ICallInterceptor</a>



<a href="https://msdn.microsoft.com/66de8d71-c27c-41bd-a741-02de5c779290">ICallUnmarshal</a>



<a href="https://msdn.microsoft.com/01773aa6-3eb5-43dd-8a10-d1351a07fe1f">ISurrogateService</a>
 

 

