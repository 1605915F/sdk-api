---
UID: NF:shobjidl_core.IFolderView2.GetSortColumns
title: IFolderView2::GetSortColumns (shobjidl_core.h)
author: windows-sdk-content
description: Gets the sort columns currently applied to the view.
old-location: shell\IFolderView2_GetSortColumns.htm
tech.root: shell
ms.assetid: 33d005bd-3ea0-42d0-ae87-417fb7c087d4
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSortColumns, GetSortColumns method [Windows Shell], GetSortColumns method [Windows Shell],IFolderView2 interface, IFolderView2 interface [Windows Shell],GetSortColumns method, IFolderView2.GetSortColumns, IFolderView2::GetSortColumns, _shell_IFolderView2_GetSortColumns, shell.IFolderView2_GetSortColumns, shobjidl_core/IFolderView2::GetSortColumns
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - IFolderView2.GetSortColumns
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFolderView2::GetSortColumns


## -description


Gets the sort columns currently applied to the view.


## -parameters




### -param rgSortColumns [out]

Type: <b>const <a href="https://msdn.microsoft.com/3ca4c318-6462-4e22-813c-ef7b3ef03230">SORTCOLUMN</a>*</b>

A pointer to a <a href="https://msdn.microsoft.com/3ca4c318-6462-4e22-813c-ef7b3ef03230">SORTCOLUMN</a> structure. The size of this structure is determined by <i>cColumns</i>.


### -param cColumns [in]

Type: <b>int</b>

The count of columns to sort by.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



