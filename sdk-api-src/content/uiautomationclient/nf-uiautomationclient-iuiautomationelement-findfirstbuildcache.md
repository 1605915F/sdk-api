---
UID: NF:uiautomationclient.IUIAutomationElement.FindFirstBuildCache
title: IUIAutomationElement::FindFirstBuildCache
author: windows-sdk-content
description: Retrieves the first child or descendant element that matches the specified condition, prefetches the requested properties and control patterns, and stores the prefetched items in the cache.
old-location: winauto\uiauto_IUIAutomationElement_FindFirstBuildCache.htm
tech.root: WinAuto
ms.assetid: ecb10fbf-ff1d-4bd0-b036-1050560d82fe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FindFirstBuildCache, FindFirstBuildCache method [Windows Accessibility], FindFirstBuildCache method [Windows Accessibility],IUIAutomationElement interface, IUIAutomationElement interface [Windows Accessibility],FindFirstBuildCache method, IUIAutomationElement.FindFirstBuildCache, IUIAutomationElement::FindFirstBuildCache, uiauto.uiauto_IUIAutomationElement_FindFirstBuildCache, uiauto_IUIAutomationElement_FindFirstBuildCache, uiautomationclient/IUIAutomationElement::FindFirstBuildCache, winauto.uiauto_IUIAutomationElement_FindFirstBuildCache
ms.topic: method
req.header: uiautomationclient.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista, Windows XP with SP3 and Platform Update for Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008, Windows Server 2003 with SP2 and Platform Update for Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAutomationClient.idl
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
 - UIAutomationClient.h
api_name:
 - IUIAutomationElement.FindFirstBuildCache
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAutomationElement::FindFirstBuildCache


## -description


Retrieves the first child or descendant element that matches the specified condition, prefetches the requested properties and control patterns, and stores the prefetched items in the cache.


## -parameters




### -param arg1 [in]

Type: <b><a href="https://msdn.microsoft.com/eb9e05b3-bcfa-4fed-9cc9-6ea8a778618e">TreeScope</a></b>

A combination of values specifying the scope of the search.


### -param condition [in]

Type: <b><a href="https://msdn.microsoft.com/66515d42-2b98-4923-b326-9fec557345b7">IUIAutomationCondition</a>*</b>

A pointer to a condition that represents the criteria to match.


### -param cacheRequest [in]

Type: <b><a href="https://msdn.microsoft.com/8e5d7f6e-c4c7-4bb9-ba33-959e098ecd41">IUIAutomationCacheRequest</a>*</b>

A pointer to a cache request that specifies the control patterns and properties to include in the cache.


### -param found [out, retval]

Type: <b><a href="https://msdn.microsoft.com/9e1f87b1-a204-4ca9-acf2-a40277012207">IUIAutomationElement</a>**</b>

Receives a pointer to the matching element, or <b>NULL</b> if no matching element is found.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The scope of the search is relative to the element on which the method is called. Elements are returned in the order in which they were encountered in the tree.

This function cannot search for ancestor elements in the Microsoft UI Automation tree; that is, <a href="https://msdn.microsoft.com/en-us/library/Ee671699(v=VS.85).aspx">TreeScope_Ancestors</a>  is not a valid value for the <i>scope</i> parameter.

When searching for top-level windows on the desktop, be sure to specify <a href="https://msdn.microsoft.com/en-us/library/Ee671699(v=VS.85).aspx">TreeScope_Children</a> in the <i>scope</i> parameter, not <a href="https://msdn.microsoft.com/en-us/library/Ee671699(v=VS.85).aspx">TreeScope_Descendants</a>. A search through the entire subtree of the desktop could iterate through thousands of items and lead to a stack overflow.

If your client application might try to find elements in its own user interface, you must make all UI Automation calls on a separate thread.

To search the raw tree, specify the appropriate <a href="https://msdn.microsoft.com/eb9e05b3-bcfa-4fed-9cc9-6ea8a778618e">TreeScope</a> in the <i>cacheRequest</i> parameter.




## -see-also




<a href="https://msdn.microsoft.com/948b3bb9-75a9-4197-9680-e6fe7bb86feb">Caching UI Automation Properties and Control Patterns</a>



<b>Conceptual</b>



<a href="https://msdn.microsoft.com/ead73c6d-7fb8-4e00-b027-5d747268af08">FindAll</a>



<a href="https://msdn.microsoft.com/acf16f88-2b68-4fd4-b715-b3a61340bdd0">FindAllBuildCache</a>



<a href="https://msdn.microsoft.com/84098431-46e8-49bd-a258-337ad1d68f91">FindFirst</a>



<a href="https://msdn.microsoft.com/9e1f87b1-a204-4ca9-acf2-a40277012207">IUIAutomationElement</a>



<a href="https://msdn.microsoft.com/8675851a-4a72-4cbe-ab71-ed6fc891be17">Obtaining UI Automation Elements</a>



<b>Reference</b>
 

 

