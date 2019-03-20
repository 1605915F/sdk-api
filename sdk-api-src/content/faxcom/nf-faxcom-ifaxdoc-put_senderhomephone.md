---
UID: NF:faxcom.IFaxDoc.put_SenderHomePhone
title: IFaxDoc::put_SenderHomePhone (faxcom.h)
author: windows-sdk-content
description: Sets or retrieves the SenderHomePhone property of a FaxDoc object. The SenderHomePhone property is a null-terminated string that contains the home telephone number of the sender of the fax transmission.
old-location: fax\_mfax_ifaxdoc_mfax_ifaxdoc_get_senderhomephone_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_93l1.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxDoc interface [Fax Service],SenderHomePhone property, IFaxDoc.SenderHomePhone, IFaxDoc.put_SenderHomePhone, IFaxDoc::SenderHomePhone, IFaxDoc::get_SenderHomePhone, IFaxDoc::put_SenderHomePhone, SenderHomePhone property [Fax Service], SenderHomePhone property [Fax Service],IFaxDoc interface, _mfax_ifaxdoc_get_senderhomephone, fax._mfax_ifaxdoc_get_senderhomephone, fax._mfax_ifaxdoc_mfax_ifaxdoc_get_senderhomephone_cpp, faxcom/IFaxDoc::SenderHomePhone, faxcom/IFaxDoc::get_SenderHomePhone, faxcom/IFaxDoc::put_SenderHomePhone, put_SenderHomePhone
ms.topic: method
req.header: faxcom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
req.dll: Faxcom.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Faxcom.dll
api_name:
 - IFaxDoc.SenderHomePhone
 - IFaxDoc.get_SenderHomePhone
 - IFaxDoc.put_SenderHomePhone
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxDoc::put_SenderHomePhone


## -description


Sets or retrieves the <b>SenderHomePhone</b> property of a <a href="https://msdn.microsoft.com/en-us/library/ms692317(v=VS.85).aspx">FaxDoc</a> object. The <b>SenderHomePhone</b> property is a null-terminated string that contains the home telephone number of the sender of the fax transmission.

This property is read/write.


## -parameters


## -remarks



The fax sender's home telephone number can appear on the cover page.

The <b>get_SenderHomePhone</b> method allocates the memory required for the buffer pointed to by the <i>pVal</i> parameter. The client application must call the <a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a> function to deallocate the resources associated with this parameter. For more information, see <a href="https://msdn.microsoft.com/en-us/library/ms690878(v=VS.85).aspx">Freeing Fax Resources</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691931(v=VS.85).aspx">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692281(v=VS.85).aspx">IFaxDoc</a>



<a href="https://msdn.microsoft.com/en-us/library/ms221481(v=VS.85).aspx">SysFreeString</a>
 

 

