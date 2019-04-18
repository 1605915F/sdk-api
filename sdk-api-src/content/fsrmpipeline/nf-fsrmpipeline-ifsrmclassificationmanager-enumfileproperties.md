---
UID: NF:fsrmpipeline.IFsrmClassificationManager.EnumFileProperties
title: IFsrmClassificationManager::EnumFileProperties (fsrmpipeline.h)
author: windows-sdk-content
description: Enumerates the properties of the specified file.
old-location: fsrm\ifsrmclassificationmanager_enumfileproperties.htm
tech.root: fsrm
ms.assetid: 9a833e94-d26b-4c94-bf2f-76ac6db3f8e9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EnumFileProperties, EnumFileProperties method [File Server Resource Manager], EnumFileProperties method [File Server Resource Manager],FsrmClassificationManager class, EnumFileProperties method [File Server Resource Manager],IFsrmClassificationManager interface, EnumFileProperties method [File Server Resource Manager],IFsrmClassificationManager2 interface, FsrmClassificationManager class [File Server Resource Manager],EnumFileProperties method, IFsrmClassificationManager interface [File Server Resource Manager],EnumFileProperties method, IFsrmClassificationManager.EnumFileProperties, IFsrmClassificationManager2 interface [File Server Resource Manager],EnumFileProperties method, IFsrmClassificationManager2::EnumFileProperties, IFsrmClassificationManager::EnumFileProperties, fs.ifsrmclassificationmanager_enumfileproperties, fsrm.ifsrmclassificationmanager_enumfileproperties, fsrmpipeline/IFsrmClassificationManager2::EnumFileProperties, fsrmpipeline/IFsrmClassificationManager::EnumFileProperties
ms.topic: method
req.header: fsrmpipeline.h
req.include-header: FsrmPipeline.h, FsrmTlb.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2008 R2
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
req.dll: SrmSvc.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - SrmSvc.dll
api_name:
 - IFsrmClassificationManager.EnumFileProperties
 - IFsrmClassificationManager2.EnumFileProperties
 - FsrmClassificationManager.EnumFileProperties
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFsrmClassificationManager::EnumFileProperties


## -description


Enumerates the properties of the specified file.


## -parameters




### -param filePath [in]

The file that contains the properties that you want to enumerate. You must specify an absolute path to the 
      file. You cannot specify a file share.


### -param options [in]

The option to use for enumerating the file's properties. For possible values, see the 
      <a href="https://msdn.microsoft.com/d909e244-344f-4da9-987c-de406c2dc359">FsrmGetFilePropertyOptions</a> enumeration.


### -param fileProperties [out]

An <a href="https://msdn.microsoft.com/6a0c5d8b-5fed-4c55-971c-43430e3c6a8d">IFsrmCollection</a> interface that contains a 
      collection of file properties. Each item in the collection is a <b>VARIANT</b> of type 
      <b>VT_DISPATCH</b>. Query the <b>pdispVal</b> member of the variant for 
      the <a href="https://msdn.microsoft.com/feffccd1-cf72-45c0-97b3-d6efd736223e">IFsrmProperty</a> interface.


## -returns



The method returns the following return values.




## -remarks



FSRM asks the specified storage modules (see the <i>options</i> parameter) to return all 
    the properties for the file for which they are responsible. For storage modules that embed the properties in the 
    file, the list will include all properties embedded in the file (not just those defined by FSRM).

If the <i>options</i> parameter is set to 
    <b>FsrmGetFilePropertyOptions_None</b>, FSRM reruns classification on the file to ensure the 
    correct value is returned.


#### Examples

For examples in C# and PowerShell see 
     <a href="https://msdn.microsoft.com/E057898F-72A0-4AB0-BE88-4C1BE6B2B5DE">Accessing Classification Properties</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/4a8e0426-792d-49d8-acf3-ab00480e24ac">FsrmClassificationManager</a>



<a href="https://msdn.microsoft.com/cc504f6c-00d7-4f9d-9688-1c29b5066ce6">IFsrmClassificationManager</a>



<a href="https://msdn.microsoft.com/6ff821e3-f0bd-4c66-8ced-edbbfbc8503b">IFsrmClassificationManager2</a>



<a href="https://msdn.microsoft.com/bac42416-0757-462f-8869-339655f48587">IFsrmClassificationManager::ClearFileProperty</a>



<a href="https://msdn.microsoft.com/c8a3c4cb-4753-495b-88f4-2d6cdfef7dc7">IFsrmClassificationManager::GetFileProperty</a>



<a href="https://msdn.microsoft.com/0f13f00e-6ca2-4436-822e-01eff638c446">IFsrmClassificationManager::SetFileProperty</a>



<a href="https://msdn.microsoft.com/79571ae1-726e-491b-b41e-6cd10cdf3936">MSFT_FSRMClassification</a>
 

 

