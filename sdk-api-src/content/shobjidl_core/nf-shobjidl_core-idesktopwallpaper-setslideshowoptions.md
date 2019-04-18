---
UID: NF:shobjidl_core.IDesktopWallpaper.SetSlideshowOptions
title: IDesktopWallpaper::SetSlideshowOptions (shobjidl_core.h)
author: windows-sdk-content
description: Sets the desktop wallpaper slideshow settings for shuffle and timing.
old-location: shell\IDesktopWallpaper_SetSlideshowOptions.htm
tech.root: shell
ms.assetid: B3106354-C321-4770-834F-D2EF790AE114
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DSO_SHUFFLEIMAGES, IDesktopWallpaper interface [Windows Shell],SetSlideshowOptions method, IDesktopWallpaper.SetSlideshowOptions, IDesktopWallpaper::SetSlideshowOptions, SetSlideshowOptions, SetSlideshowOptions method [Windows Shell], SetSlideshowOptions method [Windows Shell],IDesktopWallpaper interface, shell.IDesktopWallpaper_SetSlideshowOptions, shobjidl_core/IDesktopWallpaper::SetSlideshowOptions
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - IDesktopWallpaper.SetSlideshowOptions
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDesktopWallpaper::SetSlideshowOptions


## -description


Sets the desktop wallpaper slideshow settings for shuffle and timing.


## -parameters




### -param options [in]

Set to either 0 to disable shuffle or the following value.



#### DSO_SHUFFLEIMAGES (0x01)

Enable shuffle; advance through the slideshow in a random order.


### -param slideshowTick [in]

The amount of time, in milliseconds, between image transitions.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/A83903B5-314B-4a8b-8D37-F8A8995DE0CB">IDesktopWallpaper</a>



<a href="https://msdn.microsoft.com/2EB99E61-F5B4-4f07-8A87-793BE59D309B">IDesktopWallpaper::GetSlideshowOptions</a>
 

 

