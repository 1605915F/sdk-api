---
UID: NF:resapi.ResUtilVerifyPrivatePropertyList
title: ResUtilVerifyPrivatePropertyList function
author: windows-sdk-content
description: Verifies that a property list is correctly formatted.
old-location: mscs\resutilverifyprivatepropertylist.htm
tech.root: mscs
ms.assetid: 3d2eaa83-dd82-4023-8466-0131f7b90abc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PRESUTIL_VERIFY_PRIVATE_PROPERTY_LIST, PRESUTIL_VERIFY_PRIVATE_PROPERTY_LIST function [Failover Cluster], ResUtilVerifyPrivatePropertyList, ResUtilVerifyPrivatePropertyList function [Failover Cluster], _wolf_resutilverifyprivatepropertylist, mscs.resutilverifyprivatepropertylist, resapi/PRESUTIL_VERIFY_PRIVATE_PROPERTY_LIST, resapi/ResUtilVerifyPrivatePropertyList
ms.topic: function
req.header: resapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Enterprise, Windows Server 2008 Datacenter
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: ResUtils.lib
req.dll: ResUtils.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - ResUtils.dll
api_name:
 - ResUtilVerifyPrivatePropertyList
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResUtilVerifyPrivatePropertyList function


## -description


Verifies that a  <a href="https://msdn.microsoft.com/57312b32-01cf-48e8-b61f-6095e23bb580">property list</a> is correctly formatted.


## -parameters




### -param pInPropertyList [in]

Pointer to an input buffer containing the property list to verify.


### -param cbInPropertyListSize [in]

Size of the input buffer pointed to by <i>pInPropertyList</i>.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>.




## -see-also




<a href="https://msdn.microsoft.com/18bc7455-a004-4aff-bf33-0edcb96e0cb0">ResUtilSetPrivatePropertyList</a>
 

 

