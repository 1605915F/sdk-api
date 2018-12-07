---
UID: NF:commoncontrols.IImageList.Draw
title: IImageList::Draw
author: windows-sdk-content
description: Draws an image list item in the specified device context.
old-location: controls\IImageList_Draw.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\imagelist\ifaces\iimagelist\draw.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Draw, Draw method [Windows Controls], Draw method [Windows Controls],IImageList interface, IImageList interface [Windows Controls],Draw method, IImageList.Draw, IImageList::Draw, comctl_IImageList_Draw, comctl_IImageList_Draw_cpp, commoncontrols/IImageList::Draw, controls.IImageList_Draw, controls.comctl_IImageList_Draw
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: commoncontrols.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: CommonControls.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Comctl32.dll (version 6.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Comctl32.dll
api_name:
 - IImageList.Draw
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IImageList::Draw


## -description


Draws an image list item in the specified device context.
		


## -parameters




### -param pimldp [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb761395(v=VS.85).aspx">IMAGELISTDRAWPARAMS</a>*</b>

A pointer to an  <a href="https://msdn.microsoft.com/en-us/library/Bb761395(v=VS.85).aspx">IMAGELISTDRAWPARAMS</a> structure that contains the  drawing parameters.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Overlay images draw transparently over the primary image specified in the <b>i</b> parameter of <a href="https://msdn.microsoft.com/en-us/library/Bb761395(v=VS.85).aspx">IMAGELISTDRAWPARAMS</a>. You specify an overlay image in the <b>fStyle</b>, parameter of <b>IMAGELISTDRAWPARAMS</b> using the <a href="https://msdn.microsoft.com/en-us/library/Bb761408(v=VS.85).aspx">INDEXTOOVERLAYMASK</a> macro to shift the one-based index of the overlay image. Use the OR operator to combine the macro's return value with the drawing style flags specified in <b>fStyle</b>. You must first specify this image as an overlay image by using <a href="https://msdn.microsoft.com/en-us/library/Bb761508(v=VS.85).aspx">IImageList::SetOverlayImage</a>. 
		

To use <b>IImageList::Draw</b>, specify Comctl32.dll version 6 in the manifest. For more information on manifests, see <a href="https://msdn.microsoft.com/en-us/library/Bb773175(v=VS.85).aspx">Enabling Visual Styles</a>. 



