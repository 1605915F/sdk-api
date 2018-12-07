---
UID: NF:certenroll.ICspStatuses.Remove
title: ICspStatuses::Remove
author: windows-sdk-content
description: Removes an ICspStatus object from the collection by index number.
old-location: security\icspstatuses_remove_method.htm
tech.root: seccertenroll
ms.assetid: de8a2598-6108-41af-b049-3b981d880e80
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICspStatuses interface [Security],Remove method, ICspStatuses.Remove, ICspStatuses::Remove, Remove, Remove method [Security], Remove method [Security],ICspStatuses interface, certenroll/ICspStatuses::Remove, security.icspstatuses_remove_method
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: CertEnroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CertEnroll.dll
api_name:
 - ICspStatuses.Remove
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICspStatuses::Remove


## -description


The <b>Remove</b> method removes an <a href="https://msdn.microsoft.com/en-us/library/Aa376760(v=VS.85).aspx">ICspStatus</a> object from the collection by index number.


## -parameters




### -param Index [in]

A <b>LONG</b> variable that contains the index of the object to remove.


## -returns



If the function succeeds, the function returns <b>S_OK</b>.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa376760(v=VS.85).aspx">ICspStatus</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa376761(v=VS.85).aspx">ICspStatuses</a>
 

 

