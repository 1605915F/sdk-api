---
UID: NF:vfw.ICCompressorFree
title: ICCompressorFree function
author: windows-sdk-content
description: The ICCompressorFree function frees the resources in the COMPVARS structure used by other VCM functions.
old-location: multimedia\iccompressorfree.htm
tech.root: Multimedia
ms.assetid: 6d0c9a7d-6458-4330-af74-3f471555cbfc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICCompressorFree, ICCompressorFree function [Windows Multimedia], _win32_ICCompressorFree, multimedia.iccompressorfree, vfw/ICCompressorFree
ms.topic: function
req.header: vfw.h
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
req.lib: Vfw32.lib
req.dll: Msvfw32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Msvfw32.dll
api_name:
 - ICCompressorFree
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICCompressorFree function


## -description



The <b>ICCompressorFree</b> function frees the resources in the <a href="https://msdn.microsoft.com/en-us/library/Dd797797(v=VS.85).aspx">COMPVARS</a> structure used by other VCM functions.




## -parameters




### -param pc

Pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd797797(v=VS.85).aspx">COMPVARS</a> structure containing the resources to be freed.


## -returns



This function does not return a value.




## -remarks



Use this function to release the resources in the <a href="https://msdn.microsoft.com/en-us/library/Dd797797(v=VS.85).aspx">COMPVARS</a> structure after using the <a href="https://msdn.microsoft.com/4a58df6a-9ac4-44bb-8c49-338bb60193fc">ICCompressorChoose</a>, <a href="https://msdn.microsoft.com/90103468-fcdc-4c40-b328-29fe467b9039">ICSeqCompressFrameStart</a>, <a href="https://msdn.microsoft.com/6159e455-1e1a-4aa5-9d75-53cd2af2656a">ICSeqCompressFrame</a>, and <a href="https://msdn.microsoft.com/3fdcd18d-4ee7-4b5a-871d-61316c716e06">ICSeqCompressFrameEnd</a> functions.




## -see-also




<a href="https://msdn.microsoft.com/193961a5-b882-4769-bce7-a53d625fc9dd">Video Compression Functions</a>



<a href="https://msdn.microsoft.com/df876309-68d3-43a3-9d83-6fdb8f345fdc">Video Compression Manager</a>
 

 

