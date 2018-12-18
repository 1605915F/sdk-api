---
UID: NF:msiquery.MsiEnableUIPreview
title: MsiEnableUIPreview function
author: windows-sdk-content
description: The MsiEnableUIPreview function enables preview mode of the user interface to facilitate authoring of user-interface dialog boxes. This function returns a handle that should be closed using MsiCloseHandle.
old-location: setup\msienableuipreview.htm
tech.root: msi
ms.assetid: 77df6829-119d-4fe6-96b0-c75381b9de6c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MsiEnableUIPreview, MsiEnableUIPreview function, _msi_msienableuipreview, msiquery/MsiEnableUIPreview, setup.msienableuipreview
ms.topic: function
req.header: msiquery.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Installer 5.0 on Windows Server 2012, Windows 8, Windows Server 2008 R2 or Windows 7. Windows Installer 4.0 or Windows Installer 4.5 on   Windows Server 2008 or Windows Vista. Windows Installer on Windows Server 2003 or Windows XP
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
req.lib: Msi.lib
req.dll: Msi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Msi.dll
api_name:
 - MsiEnableUIPreview
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MsiEnableUIPreview function


## -description


The 
<b>MsiEnableUIPreview</b> function enables preview mode of the user interface to facilitate authoring of user-interface dialog boxes. This function returns a handle that should be closed using 
<a href="https://msdn.microsoft.com/b9e90ed4-fda8-4628-a713-67c651e1b572">MsiCloseHandle</a>.


## -parameters




### -param hDatabase [in]

Handle to the database.


### -param phPreview [out]

Pointer to a returned handle for user-interface preview capability.


## -returns



This function returns UINT.




## -remarks



Note that it is recommended to use variables of type PMSIHANDLE because the installer closes PMSIHANDLE objects as they go out of scope, whereas you must close MSIHANDLE objects by calling 
<a href="https://msdn.microsoft.com/b9e90ed4-fda8-4628-a713-67c651e1b572">MsiCloseHandle</a>. For more information see <a href="https://msdn.microsoft.com/en-us/library/Bb204770(v=VS.85).aspx">Use PMSIHANDLE instead of HANDLE</a> section in the <a href="https://msdn.microsoft.com/ff48d995-fe6f-4d1b-898d-67574ed3c5b7">Windows Installer Best Practices</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa368250(v=VS.85).aspx">User Interface Functions</a>
 

 

