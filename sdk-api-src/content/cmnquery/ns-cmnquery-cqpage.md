---
UID: NS:cmnquery._cqpage
title: CQPAGE
author: windows-sdk-content
description: Used to define a query page added to a form in the query dialog box with the CQAddPagesProc callback function.
old-location: ad\cqpage.htm
tech.root: ad
ms.assetid: 09e407a2-7a58-483d-8422-4ae40c05b742
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPCQPAGE, CQPAGE, CQPAGE structure [Active Directory], LPCQPAGE, LPCQPAGE structure pointer [Active Directory], _glines_cqpage, ad.cqpage, cmnquery/CQPAGE, cmnquery/LPCQPAGE"
ms.topic: struct
req.header: cmnquery.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Cmnquery.h
api_name:
 - CQPAGE
product: Windows
targetos: Windows
req.typenames: CQPAGE, *LPCQPAGE
req.redist: 
---

# CQPAGE structure


## -description


The <b>CQPAGE</b> structure is used to define a query page added to a form in the query dialog box with the <a href="https://msdn.microsoft.com/2b62c1aa-ace7-4083-8eb3-7c5c499762c9">CQAddPagesProc</a> callback function.


## -struct-fields




### -field cbStruct

Contains the size, in bytes, of the structure.


### -field dwFlags

Reserved. This member must be zero.


### -field pPageProc

Pointer to a query page callback function defined by the query form extension. This callback function is used to notify the extension of events in the page and takes  the form of the <a href="https://msdn.microsoft.com/11d40439-0877-4870-80f8-88026c448a32">CQPageProc</a> callback function.


### -field hInstance

Contains the instance handle of the module that contains the resources identified by the <b>idPageName</b> and <b>idPageTemplate</b> members.


### -field idPageName

Contains the identifier of the string resource in <b>hInstance</b>  used for the page title.


### -field idPageTemplate

Contains the identifier of the dialog resource in <b>hInstance</b>  used for the page dialog.


### -field pDlgProc

Pointer to the dialog box procedure. For more information, see <a href="https://msdn.microsoft.com/library/ms645469(v=VS.85).aspx">DialogProc</a>.


### -field lParam

An extension-defined 32-bit value passed in the <b>lParam</b> member of the <b>CQPAGE</b> structure passed as the <i>pPage</i> parameter in  the <a href="https://msdn.microsoft.com/11d40439-0877-4870-80f8-88026c448a32">CQPageProc</a> callback function.


## -see-also




<a href="https://msdn.microsoft.com/2b62c1aa-ace7-4083-8eb3-7c5c499762c9">CQAddPagesProc</a>



<a href="https://msdn.microsoft.com/11d40439-0877-4870-80f8-88026c448a32">CQPageProc</a>



<a href="https://msdn.microsoft.com/library/ms645469(v=VS.85).aspx">DialogProc</a>



<a href="https://msdn.microsoft.com/bf6aa066-ee7e-4b13-9a4b-1e097632ec5a">Display Structures in Active Directory Domain Services</a>



<a href="https://msdn.microsoft.com/797496fd-67db-4ec2-beec-224664d5d330">IQueryForm::AddPages</a>
 

 

