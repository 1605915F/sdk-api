---
UID: NF:shobjidl_core.INewMenuClient.SelectAndEditItem
title: INewMenuClient::SelectAndEditItem (shobjidl_core.h)
author: windows-sdk-content
description: INewMenuClient::SelectAndEditItem method
old-location: shell\INewMenuClient_SelectAndEditItem.htm
tech.root: shell
ms.assetid: f731e69f-8ff0-42ff-96f8-04236f53d962
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: INewMenuClient interface [Windows Shell],SelectAndEditItem method, INewMenuClient.SelectAndEditItem, INewMenuClient::SelectAndEditItem, NMCSAEI_EDIT, NMCSAEI_SELECT, SelectAndEditItem, SelectAndEditItem method [Windows Shell], SelectAndEditItem method [Windows Shell],INewMenuClient interface, _shell_INewMenuClient_SelectAndEditItem, shell.INewMenuClient_SelectAndEditItem, shobjidl_core/INewMenuClient::SelectAndEditItem
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
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
 - COM
api_location:
 - shobjidl_core.h
api_name:
 - INewMenuClient.SelectAndEditItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# INewMenuClient::SelectAndEditItem


## -description




## -parameters




### -param pidlItem [in]

Type: <b>PCIDLIST_ABSOLUTE</b>


### -param flags [in]

Type: <b>NMCSAEI_FLAGS</b>



#### NMCSAEI_SELECT (0x0000)

0x0000.



#### NMCSAEI_EDIT (0x0001)

0x0001.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



