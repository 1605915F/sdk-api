---
UID: NC:winbio_adapter.PIBIO_ENGINE_DISCARD_ENROLLMENT_FN
title: PIBIO_ENGINE_DISCARD_ENROLLMENT_FN
author: windows-sdk-content
description: Deletes intermediate enrollment state information from the pipeline.
old-location: secbiomet\engineadapterdiscardenrollment.htm
tech.root: SecBioMet
ms.assetid: 305540bc-e0c6-460a-a00b-c295b3d6db93
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EngineAdapterDiscardEnrollment, EngineAdapterDiscardEnrollment callback function [Windows Biometric Framework API], PIBIO_ENGINE_DISCARD_ENROLLMENT_FN, PIBIO_ENGINE_DISCARD_ENROLLMENT_FN callback, secbiomet.engineadapterdiscardenrollment, winbio_adapter/EngineAdapterDiscardEnrollment
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: winbio_adapter.h
req.include-header: Winbio_adapter.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Winbio_adapter.h
api_name:
 - EngineAdapterDiscardEnrollment
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PIBIO_ENGINE_DISCARD_ENROLLMENT_FN callback function


## -description


Called by the Windows Biometric Framework to delete intermediate enrollment state information from the pipeline.


## -parameters




### -param Pipeline [in, out]

Pointer to a <a href="https://msdn.microsoft.com/b5fc2b14-b0b6-4327-a42a-ecae41c3e12a">WINBIO_PIPELINE</a> structure associated with the biometric unit performing the operation.


## -returns



If the function succeeds, it returns S_OK. If the function fails, it must return the following <b>HRESULT</b> value to indicate the error.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>Pipeline</i> parameter cannot be <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



Your implementation of this function should not save information in the biometric unit database.


#### Examples

The following pseudocode shows one possible implementation of this function. The example does not compile. You must adapt it to suit your purpose.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>//////////////////////////////////////////////////////////////////////////////////////////
//
// EngineAdapterDiscardEnrollment
//
// Purpose:
//      Deletes intermediate enrollment state information from the pipeline.
//
// Parameters:
//      Pipeline  - Pointer to a WINBIO_PIPELINE structure associated 
//                  with the biometric unit performing the operation
// 
static HRESULT
WINAPI
EngineAdapterDiscardEnrollment(
    __inout PWINBIO_PIPELINE Pipeline
    )
{
    HRESULT hr = S_OK;

    // Verify that the Pipeline parameter is not NULL.
    if (!ARGUMENT_PRESENT(Pipeline))
    {
        hr = E_POINTER;
        goto cleanup;
    }

    // Retrieve the context from the pipeline.
    PWINBIO_ENGINE_CONTEXT context = 
           (PWINBIO_ENGINE_CONTEXT)Pipeline-&gt;EngineContext;

    // Return if an enrollment is not in progress. This example assumes that 
    // an enrollment object is part of your engine context structure.
    if (context-&gt;Enrollment.InProgress != TRUE)
    {
        hr = WINBIO_E_INVALID_DEVICE_STATE;
        goto cleanup;
    }


    // Call a custom function (_AdapterDestroyEnrollmentTemplate) to release
    // any objects attached to the enrollment object.
    _AdapterDestroyEnrollmentTemplate(
        context,
        &amp;context-&gt;Enrollment
        );

    // If the _AdapterDestroyEnrollmentTemplate function does not reset the
    // InProgress data member, reset it here.
    context-&gt;Enrollment.InProgress = FALSE;

cleanup:

    return hr;
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/5f04d912-f9bc-41d4-aa9e-b843e4b5a994">Plug-in Functions</a>
 

 

