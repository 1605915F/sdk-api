---
UID: NF:fwpmu.FwpmEngineGetSecurityInfo0
title: FwpmEngineGetSecurityInfo0 function (fwpmu.h)
author: windows-sdk-content
description: Retrieves a copy of the security descriptor for the filter engine.
old-location: fwp\fwpmenginegetsecurityinfo0.htm
tech.root: fwp
ms.assetid: a2bff3b0-efc9-4357-84e2-ceecc2d33498
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FwpmEngineGetSecurityInfo0, FwpmEngineGetSecurityInfo0 function [Filtering], fwp.fwpmenginegetsecurityinfo0, fwpmu/FwpmEngineGetSecurityInfo0
ms.topic: function
req.header: fwpmu.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Fwpuclnt.lib
req.dll: Fwpuclnt.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Fwpuclnt.dll
api_name:
 - FwpmEngineGetSecurityInfo0
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# FwpmEngineGetSecurityInfo0 function


## -description


The <b>FwpmEngineGetSecurityInfo0</b> function retrieves a copy of the security descriptor for the filter engine.


## -parameters




### -param engineHandle [in]

Type: <b>HANDLE</b>

Handle for an open session to the filter engine. Call <a href="https://msdn.microsoft.com/5165f219-f3e0-4e84-915b-75912aab02b7">FwpmEngineOpen0</a> to open a session to the filter engine.


### -param securityInfo [in]

Type: <b><a href="https://msdn.microsoft.com/e3e8b35d-9d18-4611-a898-72ca13e40d33">SECURITY_INFORMATION</a></b>

The type of security information to retrieve.


### -param sidOwner [out, optional]

Type: <b><a href="https://msdn.microsoft.com/328fba4e-e590-4174-9274-52dad58cb91f">PSID</a>*</b>

The owner security identifier (SID) in the returned security descriptor.


### -param sidGroup [out, optional]

Type: <b><a href="https://msdn.microsoft.com/328fba4e-e590-4174-9274-52dad58cb91f">PSID</a>*</b>

The primary group security identifier (SID) in the returned security descriptor.


### -param dacl [out, optional]

Type: <b><a href="https://msdn.microsoft.com/0073659f-c4d5-4aaf-aaa6-ea596d3bd8b9">PACL</a>*</b>

The discretionary access control list (DACL) in the returned security descriptor.


### -param sacl [out, optional]

Type: <b><a href="https://msdn.microsoft.com/0073659f-c4d5-4aaf-aaa6-ea596d3bd8b9">PACL</a>*</b>

The system access control list (SACL) in the returned security descriptor.


### -param securityDescriptor [out]

Type: <b><a href="https://msdn.microsoft.com/653992aa-4e32-4187-b3ac-727e82bfe0b6">PSECURITY_DESCRIPTOR</a>*</b>

The returned security descriptor.


## -returns



Type: <b>DWORD</b>

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The security descriptor was retrieved successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>FWP_E_* error code</b></dt>
<dt>0x80320001—0x80320039</dt>
</dl>
</td>
<td width="60%">
A Windows Filtering Platform (WFP) specific error. See <a href="https://msdn.microsoft.com/11f3085a-f044-4a78-b47a-59b9086562bf">WFP Error Codes</a> for details.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_* error code</b></dt>
<dt>0x80010001—0x80010122</dt>
</dl>
</td>
<td width="60%">
Failure to communicate with the remote or local firewall engine.

</td>
</tr>
</table>
 




## -remarks



The returned <i>securityDescriptor</i> parameter must be freed through a call to <a href="https://msdn.microsoft.com/ba9f8c1e-f75c-4bf0-b68b-e21a358575fc">FwpmFreeMemory0</a>. The other four (optional) returned parameters must not be freed, as they point to addresses within the <i>securityDescriptor</i> parameter.

This function behaves like the standard Win32 	<a href="https://msdn.microsoft.com/64767a6b-cd79-4e02-881a-706a078ff446">GetSecurityInfo</a> function. The caller needs the same standard access rights as described in the <b>GetSecurityInfo</b> reference topic.

<b>FwpmEngineGetSecurityInfo0</b> is a specific implementation of FwpmEngineGetSecurityInfo. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a>  for more information.


#### Examples

The following C++ example illustrates initialization of a security descriptor object using <b>FwpmEngineGetSecurityInfo0</b>.


```cpp
#include <windows.h>
#include <fwpmu.h>
#include <stdio.h>

#pragma comment(lib, "Fwpuclnt.lib")

void main()
{
    HANDLE engineHandle = NULL;
    DWORD  result = ERROR_SUCCESS;

    PSECURITY_DESCRIPTOR securityDescriptor;
    SECURITY_INFORMATION securityInfo = OWNER_SECURITY_INFORMATION;

    // Several functions that use the SECURITY_DESCRIPTOR structure require that this 
    // structure be aligned on a valid pointer boundary in memory. These boundaries 
    // vary depending on the type of processor used. 

    securityDescriptor = (PSECURITY_DESCRIPTOR) malloc(sizeof(SECURITY_DESCRIPTOR));

    result = FwpmEngineOpen0( NULL, RPC_C_AUTHN_WINNT, NULL, NULL, &engineHandle );
    if (result != ERROR_SUCCESS)
    {
        printf("FwpmEngineOpen0 failed.\n");
        return;
    }
    
    result = FwpmEngineGetSecurityInfo0(
                 engineHandle, 
                 securityInfo,
                 NULL,
                 NULL,
                 NULL,
                 NULL,
                 &securityDescriptor);

    if (result != ERROR_SUCCESS)
    {
        printf("FwpmEngineGetSecurityInfo0 failed.\n");
        return;
    }

    return;
}

```





## -see-also




<a href="https://msdn.microsoft.com/31a7f409-26c9-4804-bd74-b9ee356da84c">FwpmEngineSetSecurityInfo0</a>
 

 

