---
UID: NF:tom.ITextDocument2.GetActiveStory
title: ITextDocument2::GetActiveStory
author: windows-sdk-content
description: Gets the active story; that is, the story that receives keyboard and mouse input.
old-location: controls\itextdocument2_getactivestory.htm
tech.root: controls
ms.assetid: 9849d958-5bcf-44d9-827c-3d5619ba2357
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetActiveStory, GetActiveStory method [Windows Controls], GetActiveStory method [Windows Controls],ITextDocument2 interface, ITextDocument2 interface [Windows Controls],GetActiveStory method, ITextDocument2.GetActiveStory, ITextDocument2::GetActiveStory, controls.itextdocument2_getactivestory, tom/ITextDocument2::GetActiveStory
ms.topic: method
req.header: tom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextDocument2.GetActiveStory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextDocument2::GetActiveStory


## -description


Gets the active story; that is, the story that receives keyboard and mouse input.


## -parameters




### -param ppStory [out, retval]

Type: <b><a href="https://msdn.microsoft.com/8b52c6e8-c250-4cfb-979e-770df9f94010">ITextStory</a>**</b>

The active story.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the method succeeds, it returns <b>NOERROR</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/0b0a54d7-7606-41f6-b8be-6367d9180ef4">ITextDocument2</a>



<a href="https://msdn.microsoft.com/2c71673c-5119-4906-99e0-1a2aa04589e1">ITextDocument2::SetActiveStory</a>
 

 

