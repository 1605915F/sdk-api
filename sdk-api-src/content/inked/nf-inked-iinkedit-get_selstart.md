---
UID: NF:inked.IInkEdit.get_SelStart
title: IInkEdit::get_SelStart
author: windows-sdk-content
description: Gets or sets the starting point of the text that is selected in the InkEdit control (run time only).
old-location: tablet\inkedit_selstart.htm
tech.root: tablet
ms.assetid: 5f8925c0-ec62-425e-a020-9c534056e63f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IInkEdit interface [Tablet PC],SelStart property, IInkEdit.SelStart, IInkEdit.get_SelStart, IInkEdit::SelStart, IInkEdit::get_SelStart, IInkEdit::put_SelStart, InkEdit.get_SelStart, InkEdit.put_SelStart, SelStart property [Tablet PC], SelStart property [Tablet PC],IInkEdit interface, get_SelStart, inked/IInkEdit::SelStart, inked/IInkEdit::get_SelStart, inked/IInkEdit::put_SelStart, put_SelStart, tablet.inkedit_selstart
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: inked.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: InkEd.dll
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - InkEd.dll
 - InkEd.dll.dll
api_name:
 - IInkEdit.SelStart
 - IInkEdit.get_SelStart
 - IInkEdit.put_SelStart
 - InkEdit.get_SelStart
 - InkEdit.put_SelStart
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInkEdit::get_SelStart


## -description


Gets or sets the starting point of the text that is selected in the <a href="https://msdn.microsoft.com/a1dfa254-cade-44c5-8fdd-74bb40849063">InkEdit</a> control (run time only).

This property is read/write.


## -parameters


## -remarks



Setting <b>SelStart</b> greater than the text length sets the property to the existing text length; changing <b>SelStart</b> changes the selection to an insertion point and sets <a href="https://msdn.microsoft.com/6295a536-831e-4603-9412-87b2fa5b7f53">SelLength</a> to 0.




## -see-also




<a href="https://msdn.microsoft.com/8F47529B-52E9-4D67-81B3-DD2584B98101">IInkEdit</a>



<a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a>
 

 

