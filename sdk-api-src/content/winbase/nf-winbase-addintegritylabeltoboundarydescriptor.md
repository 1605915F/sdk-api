---
UID: NF:winbase.AddIntegrityLabelToBoundaryDescriptor
title: AddIntegrityLabelToBoundaryDescriptor function
author: windows-sdk-content
description: Adds a new required security identifier (SID) to the specified boundary descriptor.
old-location: base\addintegritylabeltoboundarydescriptor.htm
tech.root: sync
ms.assetid: 6b56e664-7795-4e30-8bca-1e4df2764606
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddIntegrityLabelToBoundaryDescriptor, AddIntegrityLabelToBoundaryDescriptor function, base.addintegritylabeltoboundarydescriptor, winbase/AddIntegrityLabelToBoundaryDescriptor
ms.topic: function
req.header: winbase.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - kernel32.dll
api_name:
 - AddIntegrityLabelToBoundaryDescriptor
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# AddIntegrityLabelToBoundaryDescriptor function


## -description


Adds a new required security identifier (SID) to the specified boundary descriptor.


## -parameters




### -param BoundaryDescriptor [in, out]

A handle to the boundary descriptor. The <a href="https://msdn.microsoft.com/c7789e90-8dfb-47ee-a0b2-906520982d84">CreateBoundaryDescriptor</a> function returns this handle.


### -param IntegrityLabel [in]

A pointer to a <a href="https://msdn.microsoft.com/328fba4e-e590-4174-9274-52dad58cb91f">SID</a> structure that represents the mandatory integrity level for the namespace. Use one of the following RID values to create the SID:

<b>SECURITY_MANDATORY_UNTRUSTED_RID</b>
<b>SECURITY_MANDATORY_LOW_RID</b>
<b>SECURITY_MANDATORY_MEDIUM_RID</b>
<b>SECURITY_MANDATORY_SYSTEM_RID</b>
<b>SECURITY_MANDATORY_PROTECTED_PROCESS_RID</b>
For more information, see <a href="https://msdn.microsoft.com/eb2f95c4-9465-409b-b76c-9ccae1d05eda">Well-Known SIDs</a>.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



A process can create a private namespace only with an integrity level that is  equal to or lower than the  current integrity level of the process. Therefore, a high integrity-level process can create a high, medium or low integrity-level namespace. A medium integrity-level process can create only a medium or low integrity-level namespace.

A process would usually specify a namespace at the same integrity level as the process for protection against squatting attacks by lower integrity-level processes. 

The security descriptor that the creator places on the namespace determines who can open the namespace. So a low or medium integrity-level process could be given permission to open a high integrity level namespace if the security descriptor of the namespace permits it.

To compile an application that uses this function, define <b>_WIN32_WINNT</b> as 0x0601 or later.




## -see-also




<a href="https://msdn.microsoft.com/c7789e90-8dfb-47ee-a0b2-906520982d84">CreateBoundaryDescriptor</a>
 

 

