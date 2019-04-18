---
UID: NF:uiautomationcore.IRangeValueProvider.get_LargeChange
title: IRangeValueProvider::get_LargeChange (uiautomationcore.h)
author: windows-sdk-content
description: Specifies the value that is added to or subtracted from the IRangeValueProvider::Value property when a large change is made, such as when the PAGE DOWN key is pressed.
old-location: winauto\uiauto_IRangeValueProvider_LargeChange.htm
tech.root: WinAuto
ms.assetid: 5f6d5a05-f91d-48ee-8782-f39661051584
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IRangeValueProvider interface [Windows Accessibility],LargeChange property, IRangeValueProvider.LargeChange, IRangeValueProvider.get_LargeChange, IRangeValueProvider::LargeChange, IRangeValueProvider::get_LargeChange, LargeChange property [Windows Accessibility], LargeChange property [Windows Accessibility],IRangeValueProvider interface, get_LargeChange, uiauto.uiauto_IRangeValueProvider_LargeChange, uiauto_IRangeValueProvider_LargeChange, uiautomationcore/IRangeValueProvider::LargeChange, uiautomationcore/IRangeValueProvider::get_LargeChange, winauto.uiauto_IRangeValueProvider_LargeChange
ms.topic: method
req.header: uiautomationcore.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAutomationCore.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Uiautomationcore.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Uiautomationcore.dll
api_name:
 - IRangeValueProvider.LargeChange
 - IRangeValueProvider.get_LargeChange
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IRangeValueProvider::get_LargeChange


## -description


Specifies the value that is added to or subtracted from the <a href="https://msdn.microsoft.com/b17ca8c8-948b-4d92-a6c7-79e610aa8e4a">IRangeValueProvider::Value</a> 
        property when a large change is made, such as when the PAGE DOWN key is pressed.
        

This property is read-only.


## -parameters


## -remarks



The LargeChange property can support Not a Number (NaN) value. When returning a NaN value, the provider should return a quiet (non-signaling) NaN to avoid raising an exception if floating-point exceptions are turned on. The following example shows how to create a quiet NaN:

            


```
ULONGLONG ulNaN = 0xFFFFFFFFFFFFFFFF;
    *pRetVal = *reinterpret_cast<double*>(&ulNaN);
```


Alternatively, you can use the following function from the standard C++ libraries:


```
numeric_limits<double>::quiet_NaN( )
```





## -see-also




<a href="https://msdn.microsoft.com/1e9e39f9-e728-4ed6-bc62-80d3bbe6302d">IRangeValueProvider</a>



<a href="https://msdn.microsoft.com/8928c889-0e0a-439f-87e8-a9d121fcf73f">UI Automation Providers Overview</a>
 

 

