---
UID: NS:appmodel.PACKAGE_VERSION
title: PACKAGE_VERSION
author: windows-sdk-content
description: Represents the package version information.
old-location: appxpkg\package_version.htm
tech.root: appxpkg
ms.assetid: 8543DF84-A908-4DF5-AEE6-169FECB2AA97
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PACKAGE_VERSION, PACKAGE_VERSION structure [App packaging and management], appmodel/PACKAGE_VERSION, appxpkg.package_version
ms.topic: struct
req.header: appmodel.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - AppModel.h
api_name:
 - PACKAGE_VERSION
product: Windows
targetos: Windows
req.typenames: PACKAGE_VERSION
req.redist: 
---

# PACKAGE_VERSION structure


## -description


Represents the package version information.


## -struct-fields




### -field DUMMYUNIONNAME

 


### -field DUMMYUNIONNAME.Version

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT64</a></b>

The full version number of the package represented as a single integral value.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME

 


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.Revision

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">USHORT</a></b>

The revision version number of the package.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.Build

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">USHORT</a></b>

The build version number of the package.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.Minor

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">USHORT</a></b>

The minor version number of the package.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.Major

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">USHORT</a></b>

The major version number of the package.


## -see-also




<a href="https://msdn.microsoft.com/4B15281A-2227-47B7-A750-0A01DB8543FC">PACKAGE_ID</a>
 

 

