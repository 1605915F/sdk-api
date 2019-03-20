---
UID: NF:oaidl.BSTR_UserSize64
title: BSTR_UserSize64 function (oaidl.h)
author: windows-sdk-content
description: Calculates the wire size of the BSTR object, and gets its handle and data.
old-location: automat\bstr_usersize64.htm
tech.root: automat
ms.assetid: 56ba0992-b5df-419d-b531-ea974413a7b0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BSTR_UserSize64, BSTR_UserSize64 function [Automation], automat.bstr_usersize64, oaidl/BSTR_UserSize64
ms.topic: function
req.header: oaidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: OleAut32.lib
req.dll: OleAut32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - OleAut32.dll
api_name:
 - BSTR_UserSize64
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# BSTR_UserSize64 function


## -description


Calculates the wire size of the <a href="https://msdn.microsoft.com/1b2d7d2c-47af-4389-a6b6-b01b7e915228">BSTR</a> object, and gets its handle and data.


## -parameters




### -param arg1 [in]

The data used by RPC.


### -param arg2 [in]

The current buffer offset where the object will be marshaled. The method has to account for any padding needed for the <a href="https://msdn.microsoft.com/1b2d7d2c-47af-4389-a6b6-b01b7e915228">BSTR</a> object to be properly aligned when it will be marshaled to the buffer.


### -param arg3 [in]

The object.


## -returns



The value obtained from the returned <b>HRESULT</b> value is <b>S_OK</b>.



