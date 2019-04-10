---
UID: NF:msdrm.DRMGetBoundLicenseObjectCount
title: DRMGetBoundLicenseObjectCount function (msdrm.h)
author: windows-sdk-content
description: Retrieves the number of occurrences of an object within a specified branch of a license.
old-location: rm\drmgetboundlicenseobjectcount.htm
tech.root: AdRms_Sdk
ms.assetid: 1bb9a9b7-f254-4c2b-a7b0-5e9b99c92488
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DRMGetBoundLicenseObjectCount, DRMGetBoundLicenseObjectCount function [Active Directory Rights Management Services SDK 1.0], msdrm/DRMGetBoundLicenseObjectCount, rm.drmgetboundlicenseobjectcount
ms.topic: function
req.header: msdrm.h
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
req.lib: Msdrm.lib
req.dll: Msdrm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Msdrm.dll
api_name:
 - DRMGetBoundLicenseObjectCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# DRMGetBoundLicenseObjectCount function


## -description


<p class="CCE_Message">[The AD RMS SDK leveraging functionality exposed by 

the client in Msdrm.dll is available for use in Windows Server 2008, Windows Vista, Windows Server 2008 R2, Windows 7, Windows Server 2012, and Windows 8. It may be altered or 

unavailable in subsequent versions. Instead, use <a href="https://msdn.microsoft.com/a7900f40-4c53-4760-8e5a-9c88149f86d0">Active Directory Rights Management Services SDK 2.1</a>, 

which leverages functionality exposed by the client in Msipc.dll.]

The <b>DRMGetBoundLicenseObjectCount</b> function retrieves the number of occurrences of an object within a specified branch of a license.


## -parameters




### -param hQueryRoot [in]

A handle to the branch of the license to query, from <a href="https://msdn.microsoft.com/d1be0668-fb5a-4541-92dc-34255ba3fdad">DRMGetBoundLicenseObject</a> or <a href="https://msdn.microsoft.com/102fa347-47be-4dc7-ba17-3f1ad3735b00">DRMCreateBoundLicense</a>.


### -param wszSubObjectType [in]

The type of XrML object to find. For more information, see Remarks.


### -param pcSubObjects [out]

Number of objects of this type within this branch.


## -returns



If the function succeeds, the function returns S_OK.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following list. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.




## -remarks



Certain license structures, such as a <b>RIGHT</b> structure, may have multiple instances in a license. This method returns a count of these occurrences, so that an application can iterate through them to access a particular one by using <a href="https://msdn.microsoft.com/d1be0668-fb5a-4541-92dc-34255ba3fdad">DRMGetBoundLicenseObject</a>.

The Active Directory Rights Management system exposes an object-oriented interface to the underlying license XrML. This function, along with other <b>DRMGetBoundLicense_xxx</b> functions, allows an application to navigate this structure. For more information, see <a href="https://msdn.microsoft.com/7496380a-2848-4353-a672-27fc5a9eed92">Querying Licenses</a>.




## -see-also




<a href="https://msdn.microsoft.com/b3b4e7c6-d3d3-4bf7-b6c4-9502a56a7223">AD RMS Functions</a>



<a href="https://msdn.microsoft.com/715fb3e6-6b1e-4136-9c25-efcde2015d6f">DRMGetBoundLicenseAttribute</a>



<a href="https://msdn.microsoft.com/5b3814f5-bab7-4b46-a38b-54406cb8cae0">DRMGetBoundLicenseAttributeCount</a>



<a href="https://msdn.microsoft.com/d1be0668-fb5a-4541-92dc-34255ba3fdad">DRMGetBoundLicenseObject</a>



<a href="https://msdn.microsoft.com/7496380a-2848-4353-a672-27fc5a9eed92">Querying Licenses</a>
 

 

