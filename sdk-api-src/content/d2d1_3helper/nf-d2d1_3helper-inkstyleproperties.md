---
UID: NF:d2d1_3helper.InkStyleProperties
title: InkStyleProperties function
author: windows-sdk-content
description: Creates a D2D1_INK_STYLE_PROPERTIES structure.
old-location: direct2d\inkstyleproperties.htm
tech.root: direct2d
ms.assetid: a923ce8e-71a0-6332-13e1-a4d58750d1ff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InkStyleProperties, InkStyleProperties function [Direct2D], d2d1_3helper/InkStyleProperties, direct2d.inkstyleproperties
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: d2d1_3helper.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D2d1.lib
req.dll: D2d1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - D2d1.dll
api_name:
 - InkStyleProperties
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# InkStyleProperties function


## -description


Creates a <a href="https://msdn.microsoft.com/en-us/library/Dn890737(v=VS.85).aspx">D2D1_INK_STYLE_PROPERTIES</a> structure.
        


## -parameters




### -param nibShape

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn890735(v=VS.85).aspx">D2D1_INK_NIB_SHAPE</a></b>

The pre-transform shape of the nib (pen tip) used to draw a given ink object.


### -param nibTransform [ref]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/Dd368132(v=VS.85).aspx">D2D1_MATRIX_3X2_F</a></b>

The transform applied to the nib. Note that the translation components of the transform matrix are ignored for the purposes of rendering.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn890737(v=VS.85).aspx">D2D1_INK_STYLE_PROPERTIES</a></b>

Returns the created <a href="https://msdn.microsoft.com/en-us/library/Dn890737(v=VS.85).aspx">D2D1_INK_STYLE_PROPERTIES</a> structure.
          




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn890737(v=VS.85).aspx">D2D1_INK_STYLE_PROPERTIES</a>
 

 

