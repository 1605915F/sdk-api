---
UID: NS:adsprop._ADSPROPERROR
title: ADSPROPERROR (adsprop.h)
author: windows-sdk-content
description: The ADSPROPERROR structure is used to pass error data to the notification object with the ADsPropSendErrorMessage function or the WM_ADSPROP_NOTIFY_ERROR message.
old-location: ad\adsproperror.htm
tech.root: ad
ms.assetid: 584cb3e7-3b26-4346-9162-b3e3064ded1a
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PADSPROPERROR, ADSPROPERROR, ADSPROPERROR structure [Active Directory], PADSPROPERROR, PADSPROPERROR structure pointer [Active Directory], _glines_adsproperror, ad.adsproperror, adsprop/ADSPROPERROR, adsprop/PADSPROPERROR"
ms.topic: struct
req.header: adsprop.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
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
 - HeaderDef
api_location:
 - Adsprop.h
api_name:
 - ADSPROPERROR
product: Windows
targetos: Windows
req.typenames: ADSPROPERROR, *PADSPROPERROR
req.redist: 
---

# ADSPROPERROR structure


## -description


The
  <b>ADSPROPERROR</b> structure is used to pass error
  data to the notification object with the <a href="https://msdn.microsoft.com/a1ca8440-0b18-4439-9143-bd8119f4f6ae">ADsPropSendErrorMessage</a> function or the <a href="https://msdn.microsoft.com/7abf1b3d-5abe-42cd-baeb-1bf863c7f04d">WM_ADSPROP_NOTIFY_ERROR</a> message.


## -struct-fields




### -field hwndPage

Contains the window handle of the property page that generated the error.


### -field pszPageTitle

Pointer to a NULL-terminated Unicode string that contains the title of the property page that generated the error.


### -field pszObjPath

Pointer to a NULL-terminated Unicode string that contains the ADsPath of the directory object that the error occurred on.


### -field pszObjClass

Pointer to a NULL-terminated Unicode string that contains the class name of the directory object that the error occurred on.


### -field hr

Contains an <b>HRESULT</b> value that specifies the  code of the error that occurred. If <i>hr</i> is not equal to <b>S_OK</b>, then <i>pszError</i> is ignored. If <i>hr</i>is equal to <b>S_OK</b>, then <i>pszError</i> contains an error message.


### -field pszError

Pointer to a NULL-terminated Unicode string that contains the error message to be displayed in the error dialog box. This member is ignored if <i>hr</i> is not equal to <b>S_OK</b>. In this case, the error dialog box will display a system-defined message for the error specified by <i>hr</i>.


## -see-also




<a href="https://msdn.microsoft.com/a1ca8440-0b18-4439-9143-bd8119f4f6ae">ADsPropSendErrorMessage</a>



<a href="https://msdn.microsoft.com/7abf1b3d-5abe-42cd-baeb-1bf863c7f04d">WM_ADSPROP_NOTIFY_ERROR</a>
 

 

