---
UID: NS:sessdirpublictypes.__MIDL___MIDL_itf_sessdirpublictypes_0000_0000_0002
title: TSSD_ConnectionPoint
author: windows-sdk-content
description: Defines the IP address of a target.
old-location: termserv\tssd_connectionpoint.htm
tech.root: TermServ
ms.assetid: 489d79ab-8a59-4789-9dca-df26018bf58c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PTSSD_ConnectionPoint, PTSSD_ConnectionPoint, PTSSD_ConnectionPoint structure pointer [Remote Desktop Services], TSSD_ConnectionPoint, TSSD_ConnectionPoint structure [Remote Desktop Services], sessdirpublictypes/PTSSD_ConnectionPoint, sessdirpublictypes/TSSD_ConnectionPoint, termserv.tssd_connectionpoint"
ms.topic: struct
req.header: sessdirpublictypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: SessDirPublicTypes.idl
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
 - SessDirPublicTypes.h
api_name:
 - TSSD_ConnectionPoint
product: Windows
targetos: Windows
req.typenames: TSSD_ConnectionPoint, *PTSSD_ConnectionPoint
req.redist: 
---

# TSSD_ConnectionPoint structure


## -description


Defines the IP address of a target.


## -struct-fields




### -field ServerAddressB

The server address.


### -field AddressType

A value of the <a href="https://msdn.microsoft.com/en-us/library/Ff678305(v=VS.85).aspx">TSSD_AddrV46Type</a> enumeration  that indicates the IP address type.


### -field PortNumber

The IP port number.


### -field AddressScope

The scope of the address.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff678305(v=VS.85).aspx">TSSD_AddrV46Type</a>
 

 

