---
UID: NF:d3d10effect.ID3D10EffectVariable.AsString
title: ID3D10EffectVariable::AsString (d3d10effect.h)
author: windows-sdk-content
description: Get a string variable.
old-location: direct3d10\id3d10effectvariable_asstring.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectvariable_asstring.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 147dcf91-ad41-9a2f-06f9-e60ddc770e29, AsString, AsString method [Direct3D 10], AsString method [Direct3D 10],ID3D10EffectVariable interface, ID3D10EffectVariable interface [Direct3D 10],AsString method, ID3D10EffectVariable.AsString, ID3D10EffectVariable::AsString, d3d10effect/ID3D10EffectVariable::AsString, direct3d10.id3d10effectvariable_asstring
ms.topic: method
req.header: d3d10effect.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - COM
api_location:
 - D3D10Effect.h
api_name:
 - ID3D10EffectVariable.AsString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10EffectVariable::AsString


## -description


Get a string variable.


## -parameters






## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173705(v=VS.85).aspx">ID3D10EffectStringVariable</a>*</b>

A pointer to a string variable. See <a href="https://msdn.microsoft.com/en-us/library/Bb173705(v=VS.85).aspx">ID3D10EffectStringVariable</a>.




## -remarks



AsString returns a version of the effect variable that has been specialized to a string variable. Similar to a cast, this specialization will return an invalid object if the effect variable does not contain string data.

Applications can test the returned object for validity by calling <a href="https://msdn.microsoft.com/en-us/library/Bb173746(v=VS.85).aspx">IsValid</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173724(v=VS.85).aspx">ID3D10EffectVariable Interface</a>
 

 

