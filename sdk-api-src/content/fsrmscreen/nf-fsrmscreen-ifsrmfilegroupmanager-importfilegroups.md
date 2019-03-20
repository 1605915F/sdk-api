---
UID: NF:fsrmscreen.IFsrmFileGroupManager.ImportFileGroups
title: IFsrmFileGroupManager::ImportFileGroups (fsrmscreen.h)
author: windows-sdk-content
description: Imports the specified file groups from an XML string.
old-location: fsrm\ifsrmfilegroupmanager_importfilegroups.htm
tech.root: fsrm
ms.assetid: 81f62d49-5fce-4d8c-96b5-506d741c5f77
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FsrmFileGroupManager class [File Server Resource Manager],ImportFileGroups method, IFsrmFileGroupManager interface [File Server Resource Manager],ImportFileGroups method, IFsrmFileGroupManager.ImportFileGroups, IFsrmFileGroupManager::ImportFileGroups, ImportFileGroups, ImportFileGroups method [File Server Resource Manager], ImportFileGroups method [File Server Resource Manager],FsrmFileGroupManager class, ImportFileGroups method [File Server Resource Manager],IFsrmFileGroupManager interface, fs.ifsrmfilegroupmanager_importfilegroups, fsrm.ifsrmfilegroupmanager_importfilegroups, fsrmscreen/IFsrmFileGroupManager::ImportFileGroups
ms.topic: method
req.header: fsrmscreen.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008
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
 - IFsrmFileGroupManager.ImportFileGroups
 - FsrmFileGroupManager.ImportFileGroups
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFsrmFileGroupManager::ImportFileGroups


## -description


<p class="CCE_Message">[This method is supported for compatibility but it's recommended to use the 
    <a href="https://msdn.microsoft.com/1CE772FA-CE33-4900-A499-058175A7C37E">FSRM WMI Classes</a> to manage FSRM. Please see the 
    <a href="https://msdn.microsoft.com/c090da1e-df74-4dba-aaa0-15defa85d604">MSFT_FSRMFileGroup</a> class.]

Imports the specified file groups from an XML string.


## -parameters




### -param serializedFileGroups [in]

An XML string that represents one or more file groups.


### -param fileGroupNamesArray [in]

A <b>VARIANT</b> that contains a <b>SAFEARRAY</b> of the names 
      of the file groups to import. If <b>NULL</b>, the method imports all file groups.


### -param fileGroups [out]

An <a href="https://msdn.microsoft.com/ef4678b4-e6b0-4044-ba11-7a3ae01ad2c7">IFsrmCommittableCollection</a> interface 
       that contains a collection of file groups.

Each item of the collection is a <b>VARIANT</b> of type 
       <b>VT_DISPATCH</b>. Query the <b>pdispVal</b> member of the variant for 
       the <a href="https://msdn.microsoft.com/fb4f6b03-01cc-4855-8bc7-de5191068040">IFsrmFileGroupImported</a> interface.

To add the file groups to FSRM, call the 
       <a href="https://msdn.microsoft.com/844cb2a5-8526-434b-af22-b1bf856ed6af">IFsrmCommittableCollection::Commit</a> 
       method.


## -returns



The method returns the following return values.




## -see-also




<a href="https://msdn.microsoft.com/d5c9c8f0-edbe-4f34-8f34-fe9d0667926e">FsrmFileGroupManager</a>



<a href="https://msdn.microsoft.com/e0a1a3d3-f683-410d-a0d9-081cd2476d1e">IFsrmFileGroupManager</a>



<a href="https://msdn.microsoft.com/c090da1e-df74-4dba-aaa0-15defa85d604">MSFT_FSRMFileGroup</a>
 

 

