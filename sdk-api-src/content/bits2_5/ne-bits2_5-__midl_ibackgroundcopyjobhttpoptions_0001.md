---
UID: NE:bits2_5.__MIDL_IBackgroundCopyJobHttpOptions_0001
title: "__MIDL_IBackgroundCopyJobHttpOptions_0001"
author: windows-sdk-content
description: The BG_CERT_STORE_LOCATION enumeration defines the location of the certificate store.
old-location: bits\bg_cert_store_location.htm
tech.root: bits
ms.assetid: 596b1ba1-6652-4c97-a44d-e8271471d864
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: BG_CERT_STORE_LOCATION, BG_CERT_STORE_LOCATION enumeration [BITS], BG_CERT_STORE_LOCATION_CURRENT_SERVICE, BG_CERT_STORE_LOCATION_CURRENT_USER, BG_CERT_STORE_LOCATION_CURRENT_USER_GROUP_POLICY, BG_CERT_STORE_LOCATION_LOCAL_MACHINE, BG_CERT_STORE_LOCATION_LOCAL_MACHINE_ENTERPRISE, BG_CERT_STORE_LOCATION_LOCAL_MACHINE_GROUP_POLICY, BG_CERT_STORE_LOCATION_SERVICES, BG_CERT_STORE_LOCATION_USERS, __MIDL_IBackgroundCopyJobHttpOptions_0001, bits.bg_cert_store_location, bits2_5/BG_CERT_STORE_LOCATION, bits2_5/BG_CERT_STORE_LOCATION_CURRENT_SERVICE, bits2_5/BG_CERT_STORE_LOCATION_CURRENT_USER, bits2_5/BG_CERT_STORE_LOCATION_CURRENT_USER_GROUP_POLICY, bits2_5/BG_CERT_STORE_LOCATION_LOCAL_MACHINE, bits2_5/BG_CERT_STORE_LOCATION_LOCAL_MACHINE_ENTERPRISE, bits2_5/BG_CERT_STORE_LOCATION_LOCAL_MACHINE_GROUP_POLICY, bits2_5/BG_CERT_STORE_LOCATION_SERVICES, bits2_5/BG_CERT_STORE_LOCATION_USERS
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: bits2_5.h
req.include-header: Bits.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bits2_5.idl
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
 - Bits2_5.h
api_name:
 - BG_CERT_STORE_LOCATION
product: Windows
targetos: Windows
req.typenames: BG_CERT_STORE_LOCATION
req.redist: 
---

# __MIDL_IBackgroundCopyJobHttpOptions_0001 enumeration


## -description


The <b>BG_CERT_STORE_LOCATION</b> enumeration defines the location of the certificate store.


## -enum-fields




### -field BG_CERT_STORE_LOCATION_CURRENT_USER

Use the current user's certificate store.


### -field BG_CERT_STORE_LOCATION_LOCAL_MACHINE

Use the local computer's certificate store.


### -field BG_CERT_STORE_LOCATION_CURRENT_SERVICE

Use the current service's certificate store.


### -field BG_CERT_STORE_LOCATION_SERVICES

Use a specific service's certificate store.


### -field BG_CERT_STORE_LOCATION_USERS

Use a specific user's certificate store.


### -field BG_CERT_STORE_LOCATION_CURRENT_USER_GROUP_POLICY

Use the current user's group policy certificate store. In a network setting, stores in this location are downloaded to the client computer from the Group Policy Template (GPT) during computer startup or user logon. 


### -field BG_CERT_STORE_LOCATION_LOCAL_MACHINE_GROUP_POLICY

Use the local computer's certificate store. In a network setting, stores in this location are downloaded to the client computer from the Group Policy Template (GPT) during computer startup or user logon.


### -field BG_CERT_STORE_LOCATION_LOCAL_MACHINE_ENTERPRISE

Use the enterprise certificate store. The enterprise store is shared across domains in the enterprise and downloaded from the global enterprise directory.


## -remarks



For more information, see <a href="https://msdn.microsoft.com/en-us/library/Aa388136(v=VS.85).aspx">System Store Locations</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa964251(v=VS.85).aspx">IBackgroundCopyJobHttpOptions::GetClientCertificate</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa964256(v=VS.85).aspx">IBackgroundCopyJobHttpOptions::SetClientCertificateByID</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa964257(v=VS.85).aspx">IBackgroundCopyJobHttpOptions::SetClientCertificateByName</a>
 

 

