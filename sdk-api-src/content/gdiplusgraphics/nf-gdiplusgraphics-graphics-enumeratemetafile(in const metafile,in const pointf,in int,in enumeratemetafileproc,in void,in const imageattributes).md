---
UID: NF:gdiplusgraphics.Graphics.EnumerateMetafile(IN const Metafile,IN const PointF,IN INT,IN EnumerateMetafileProc,IN VOID,IN const ImageAttributes)
title: Graphics::EnumerateMetafile(IN const Metafile,IN const PointF,IN INT,IN EnumerateMetafileProc,IN VOID,IN const ImageAttributes)
author: windows-sdk-content
description: The Graphics::EnumerateMetafile method calls an application-defined callback function for each record in a specified metafile. You can use this method to display a metafile by calling PlayRecord in the callback function.
old-location: gdiplus\_gdiplus_CLASS_Graphics_EnumerateMetafile_Metafile_metafile_PointF_destPoints_INT_count_EnumerateMet.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\graphicsenumeratemetafilemethods\enumeratemetafile_24metafilemetafile_pointfdestpoints_intc.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnumerateMetafile, EnumerateMetafile method [GDI+], EnumerateMetafile method [GDI+],Graphics class, Graphics class [GDI+],EnumerateMetafile method, Graphics.EnumerateMetafile, Graphics.EnumerateMetafile(IN const Metafile,IN const PointF,IN INT,IN EnumerateMetafileProc,IN VOID,IN const ImageAttributes), Graphics.EnumerateMetafile(const Metafile*,const Point*,INT,EnumerateMetafileProc,VOID*,ImageAttributes*), Graphics::EnumerateMetafile, Graphics::EnumerateMetafile(IN const Metafile,IN const PointF,IN INT,IN EnumerateMetafileProc,IN VOID,IN const ImageAttributes), _gdiplus_CLASS_Graphics_EnumerateMetafile_Metafile_metafile_PointF_destPoints_INT_count_EnumerateMet, gdiplus._gdiplus_CLASS_Graphics_EnumerateMetafile_Metafile_metafile_PointF_destPoints_INT_count_EnumerateMet
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusgraphics.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
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
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gdiplus.dll
api_name:
 - Graphics.EnumerateMetafile
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Graphics::EnumerateMetafile(IN const Metafile,IN const PointF,IN INT,IN EnumerateMetafileProc,IN VOID,IN const ImageAttributes)


## -description


The <b>Graphics::EnumerateMetafile</b> method calls an application-defined callback function for each record in a specified metafile. You can use this method to display a metafile by calling 
			<a href="https://msdn.microsoft.com/a1214c49-63ff-4fac-9603-dce5240d9691">PlayRecord</a> in the callback function.


## -parameters




### -param metafile [in]

Type: <b>const <a href="https://msdn.microsoft.com/63b057de-9c4d-488e-ad07-ede52f9175a6">Metafile</a>*</b>

Pointer to a metafile to be enumerated. 


### -param destPoints [in]

Type: <b>const <a href="https://msdn.microsoft.com/8bf4d566-b061-4102-8307-218431e286f8">Point</a>*</b>

Pointer to an array of destination points. This is an array of three points that defines the destination parallelogram for the displayed metafile. 


### -param count [in]

Type: <b>INT</b>

Integer that specifies the number of points in the 
					<i>destPoints</i> array. 


### -param callback [in]

Type: <b>EnumerateMetafileProc</b>

Pointer to an application-defined callback function. The prototype for the callback function is given in Gdiplustypes.h. 


### -param callbackData [in]

Type: <b>VOID*</b>

Optional. Pointer to a block of data that is passed to the callback function. The default value is <b>NULL</b>. 


### -param imageAttributes [in]

Type: <b><a href="https://msdn.microsoft.com/fbb107d2-b079-4916-89bb-d61fcd860894">ImageAttributes</a>*</b>

Optional. Pointer to an 
					<a href="https://msdn.microsoft.com/fbb107d2-b079-4916-89bb-d61fcd860894">ImageAttributes</a> object that specifies color adjustments for the displayed metafile. The default value is <b>NULL</b>. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Ok</a>, which is an element of the 
						<b>Status</b> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.



