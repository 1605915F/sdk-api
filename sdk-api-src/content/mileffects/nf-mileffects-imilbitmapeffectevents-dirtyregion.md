---
UID: NF:mileffects.IMILBitmapEffectEvents.DirtyRegion
title: IMILBitmapEffectEvents::DirtyRegion (mileffects.h)
author: windows-sdk-content
description: Invalidates the specified region of the given IMILBitmapEffectPrimitive.
old-location: wibe\_wibe_imilbitmapeffectevents_dirtyregion.htm
tech.root: wibe
ms.assetid: VS|wibe|~\wibelh\reference\ifaces\imilbitmapeffectevents\dirtyregion.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DirtyRegion, DirtyRegion method [WPF Bitmap Effects], DirtyRegion method [WPF Bitmap Effects],IMILBitmapEffectEvents interface, IMILBitmapEffectEvents interface [WPF Bitmap Effects],DirtyRegion method, IMILBitmapEffectEvents.DirtyRegion, IMILBitmapEffectEvents::DirtyRegion, _wibe_imilbitmapeffectevents_dirtyregion, mileffects/IMILBitmapEffectEvents::DirtyRegion, wibe._wibe_imilbitmapeffectevents_dirtyregion
ms.topic: method
req.header: mileffects.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mileffects.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Mileffects.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mileffects.dll
api_name:
 - IMILBitmapEffectEvents.DirtyRegion
product: Windows
targetos: Windows
req.typenames: 
req.redist: Microsoft .Net 3.0
ms.custom: 19H1
---

# IMILBitmapEffectEvents::DirtyRegion


## -description


Invalidates the specified region of the given <a href="https://msdn.microsoft.com/en-us/library/ms735258(v=VS.85).aspx">IMILBitmapEffectPrimitive</a>.


## -parameters




### -param pEffect [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms735317(v=VS.85).aspx">IMILBitmapEffect</a>*</b>

A pointer to the primitive to dirty.


### -param pRect [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms735228(v=VS.85).aspx">MIL_RECTD</a>*</b>

A pointer to the rectangle to dirty.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



