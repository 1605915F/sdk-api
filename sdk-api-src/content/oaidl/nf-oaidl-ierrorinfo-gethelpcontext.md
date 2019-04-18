---
UID: NF:oaidl.IErrorInfo.GetHelpContext
title: IErrorInfo::GetHelpContext (oaidl.h)
author: windows-sdk-content
description: Returns the Help context identifier (ID) for the error.
old-location: automat\ierrorinfo_gethelpcontext.htm
tech.root: automat
ms.assetid: aadfc151-50ed-4a31-b53a-ff9d74dceb6b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetHelpContext, GetHelpContext method [Automation], GetHelpContext method [Automation],IErrorInfo interface, IErrorInfo interface [Automation],GetHelpContext method, IErrorInfo.GetHelpContext, IErrorInfo::GetHelpContext, _oa96_IErrorInfo_GetHelpContext, automat.ierrorinfo_gethelpcontext, oaidl/IErrorInfo::GetHelpContext
ms.topic: method
req.header: oaidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OaIdl.idl
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
 - oaidl.h
api_name:
 - IErrorInfo.GetHelpContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IErrorInfo::GetHelpContext


## -description


Returns the Help context identifier (ID) for the error.


## -parameters




### -param pdwHelpContext [out]

The Help context ID for the error.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This method returns the Help context ID for the error. To find the Help file to which it applies, use <a href="https://msdn.microsoft.com/f8458382-0af7-4a9b-add3-9c99af070be4">IErrorInfo::GetHelpFile</a>.





## -see-also




<a href="https://msdn.microsoft.com/4dda6909-2d9a-4727-ae0c-b5f90dcfa447">IErrorInfo</a>
 

 

