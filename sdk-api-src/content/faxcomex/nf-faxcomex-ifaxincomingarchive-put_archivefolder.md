---
UID: NF:faxcomex.IFaxIncomingArchive.put_ArchiveFolder
title: IFaxIncomingArchive::put_ArchiveFolder (faxcomex.h)
author: windows-sdk-content
description: The ArchiveFolder property is a null-terminated string that specifies the folder location on the fax server for archived inbound faxes.
old-location: fax\_mfax_faxincomingarchive_cpp_mfax_faxincomingarchive_archivefolder_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_7vle.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ArchiveFolder property [Fax Service], ArchiveFolder property [Fax Service],IFaxIncomingArchive interface, IFaxIncomingArchive interface [Fax Service],ArchiveFolder property, IFaxIncomingArchive.ArchiveFolder, IFaxIncomingArchive.put_ArchiveFolder, IFaxIncomingArchive::ArchiveFolder, IFaxIncomingArchive::get_ArchiveFolder, IFaxIncomingArchive::put_ArchiveFolder, _mfax_faxincomingarchive.archivefolder, fax._mfax_faxincomingarchive_archivefolder, fax._mfax_faxincomingarchive_cpp_mfax_faxincomingarchive_archivefolder_cpp, faxcomex/IFaxIncomingArchive::ArchiveFolder, faxcomex/IFaxIncomingArchive::get_ArchiveFolder, faxcomex/IFaxIncomingArchive::put_ArchiveFolder, put_ArchiveFolder
ms.topic: method
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxIncomingArchive.ArchiveFolder
 - IFaxIncomingArchive.get_ArchiveFolder
 - IFaxIncomingArchive.put_ArchiveFolder
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxIncomingArchive::put_ArchiveFolder


## -description


The <b>ArchiveFolder</b> property is a null-terminated string that specifies the folder location on the fax server for archived inbound faxes.

This property is read/write.


## -parameters


## -remarks



<div class="alert"><b>Note</b>  This property is not supported in Windows Vista, Windows Server 2008, and later versions of Windows. To access this property in Windows Vista, Windows Server 2008, and later versions of Windows,  get the <a href="https://msdn.microsoft.com/en-us/library/ms693549(v=VS.85).aspx">IFaxConfiguration</a> interface from the <a href="https://msdn.microsoft.com/en-us/library/Aa358976(v=VS.85).aspx">IFaxServer2</a> interface, and then call the  <a href="https://msdn.microsoft.com/en-us/library/Aa358915(v=VS.85).aspx">IFaxConfiguration::put_ArchiveLocation</a>   or <a href="https://msdn.microsoft.com/en-us/library/Aa358915(v=VS.85).aspx">IFaxConfiguration::get_ArchiveLocation</a> method.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms687473(v=VS.85).aspx">FaxIncomingArchive</a>



<a href="https://msdn.microsoft.com/en-us/library/ms687474(v=VS.85).aspx">IFaxIncomingArchive</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692976(v=VS.85).aspx">Visual Basic Example</a>
 

 

