---
UID: NE:dvdmedia.__unnamed_enum_3
title: AM_DVDCOPYSTATE (dvdmedia.h)
author: windows-sdk-content
description: Specifies the copy protection state.
old-location: dshow\am_dvdcopystate.htm
tech.root: DirectShow
ms.assetid: 32a9783e-f9f1-4e37-8cd2-3ff5634d75f6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: AM_DVDCOPYSTATE, AM_DVDCOPYSTATE enumeration [DirectShow], AM_DVDCOPYSTATE_AUTHENTICATION_NOT_REQUIRED, AM_DVDCOPYSTATE_AUTHENTICATION_REQUIRED, AM_DVDCOPYSTATE_DONE, AM_DVDCOPYSTATE_INITIALIZE, AM_DVDCOPYSTATE_INITIALIZE_TITLE, dshow.am_dvdcopystate, dvdmedia/AM_DVDCOPYSTATE, dvdmedia/AM_DVDCOPYSTATE_AUTHENTICATION_NOT_REQUIRED, dvdmedia/AM_DVDCOPYSTATE_AUTHENTICATION_REQUIRED, dvdmedia/AM_DVDCOPYSTATE_DONE, dvdmedia/AM_DVDCOPYSTATE_INITIALIZE, dvdmedia/AM_DVDCOPYSTATE_INITIALIZE_TITLE
ms.topic: enum
req.header: dvdmedia.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Dvdmedia.h
api_name:
 - AM_DVDCOPYSTATE
product: Windows
targetos: Windows
req.typenames: AM_DVDCOPYSTATE
req.redist: 
---

# AM_DVDCOPYSTATE enumeration


## -description



Specifies the copy protection state.




## -enum-fields




### -field AM_DVDCOPYSTATE_INITIALIZE

Starting a full key-exchange algorithm.


### -field AM_DVDCOPYSTATE_INITIALIZE_TITLE

Starting a title key-exchange algorithm.


### -field AM_DVDCOPYSTATE_AUTHENTICATION_NOT_REQUIRED

Authentication is not required.  


### -field AM_DVDCOPYSTATE_AUTHENTICATION_REQUIRED

Authentication required.


### -field AM_DVDCOPYSTATE_DONE

Key exchange negotiation is complete.


## -remarks



The <a href="https://msdn.microsoft.com/en-us/library/Dd373463(v=VS.85).aspx">AM_DVDCOPY_SET_COPY_STATE</a> structure uses this data type.




## -see-also




<a href="https://msdn.microsoft.com/da3abefd-8f25-449d-8787-84d2cef928da">DVD Copy Protection Property Set</a>
 

 

