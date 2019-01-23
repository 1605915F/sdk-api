---
UID: NC:winbio_adapter.PIBIO_ENGINE_ATTACH_FN
title: PIBIO_ENGINE_ATTACH_FN
author: windows-sdk-content
description: Adds an engine adapter to the processing pipeline of the biometric unit.
old-location: secbiomet\engineadapterattach.htm
tech.root: SecBioMet
ms.assetid: e797952b-c7dd-41ad-9536-97d7ce1a7a5d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EngineAdapterAttach, EngineAdapterAttach callback function [Windows Biometric Framework API], PIBIO_ENGINE_ATTACH_FN, PIBIO_ENGINE_ATTACH_FN callback, secbiomet.engineadapterattach, winbio_adapter/EngineAdapterAttach
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
 - EngineAdapterAttach
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PIBIO_ENGINE_ATTACH_FN callback function


## -description


Called by the Windows Biometric Framework when an engine adapter is added to the processing pipeline of the biometric unit. The purpose of this function is to  perform any initialization required for later biometric operations.


## -parameters




### -param Pipeline [in, out]

Pointer to a <a href="https://msdn.microsoft.com/b5fc2b14-b0b6-4327-a42a-ecae41c3e12a">WINBIO_PIPELINE</a> structure associated with the biometric unit performing the operation.


## -returns



If the function succeeds, it returns S_OK. If the function fails, it must return one of the following <b>HRESULT</b> values to indicate the error.

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
The <i>Pipeline</i> argument cannot be <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
The operation could not be completed because of insufficient memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WINBIO_E_INVALID_DEVICE_STATE</b></dt>
</dl>
</td>
<td width="60%">
The <b>EngineContext</b> member of the <a href="https://msdn.microsoft.com/b5fc2b14-b0b6-4327-a42a-ecae41c3e12a">WINBIO_PIPELINE</a> structure pointed to by the <i>Pipeline</i> argument is not <b>NULL</b> or the <b>EngineHandle</b> member is not set to <b>INVALID_HANDLE_VALUE</b>.

</td>
</tr>
</table>
 




## -remarks



This function is called before the storage adapter has been initialized for the biometric unit. Therefore, this function must not call any functions referenced by the <a href="https://msdn.microsoft.com/en-us/library/Dd401661(v=VS.85).aspx">WINBIO_STORAGE_INTERFACE</a> structure pointed to by the <b>StorageInterface</b> member of the pipeline object.

When implementing this function, you must allocate and manage any resources required by the adapter and attach these to the biometric unit pipeline. To do this, allocate a private <b>WINBIO_ENGINE_CONTEXT</b> structure on the  heap, initialize it, and set its address in the <b>EngineContext</b> member of the pipeline object.

If there is an error during the creation and initialization of engine adapter resources used by this function, you must perform any required cleanup before returning.

If the <b>EngineContext</b> field is not <b>NULL</b> when this function is called, the pipeline was not properly initialized and you must return <b>WINBIO_E_INVALID_DEVICE_STATE</b> to notify the Windows Biometric Framework of the problem.

Similarly, if the <b>EngineHandle</b> field does not contain <b>INVALID_HANDLE_VALUE</b> when this function is called, you must return <b>WINBIO_E_INVALID_DEVICE_STATE</b>.


#### Examples

The following pseudocode shows one possible implementation of this function. The example does not compile. You must adapt it to suit your purpose.


```cpp
//////////////////////////////////////////////////////////////////////////////////////////
//
// EngineAdapterAttach
//
// Purpose:
//      Performs any initialization required for later biometric operations.
//
// Parameters:
//      Pipeline -  Pointer to a WINBIO_PIPELINE structure associated with 
//                  the biometric unit performing the operation.
//
static HRESULT
WINAPI
EngineAdapterAttach(
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
    PWINBIO_ENGINE_CONTEXT newContext = NULL;

    // Call a custom function (_AdapterAlloc) to allocate memory to hold the 
    // engine adapter context.
    newContext = (PWINBIO_ENGINE_CONTEXT)_AdapterAlloc(sizeof(WINBIO_ENGINE_CONTEXT));
    if (newContext == NULL)
    {
        E_OUTOFMEMORY;
        goto cleanup;
    }

    // Clear the context memory.
    ZeroMemory(newContext, sizeof(WINBIO_ENGINE_CONTEXT));

    // Initialize any required context fields.
    newContext->SomeField = SomeSpecialValue;

    newContext->SomePointerField = _AdapterAlloc(sizeof(SOME_STRUCTURE));
    if (newContext->SomePointerField == NULL)
    {
        E_OUTOFMEMORY;
        goto cleanup;
    }

    // If your adapter supports software-based template hashing, implement the 
    // following custom function to open a SHA1 hash object handle and store 
    // the handle in the adapter context. Use Cryptography Next Generation (CNG) 
    // functions to create the SHA1 hash object.
    hr = _AdapterInitializeCrypto(newContext);
    if (FAILED(hr))
    {
        goto cleanup;
    }

    // If initialization completes successfully, attach the engine context to the 
    // processing pipeline of the biometric unit.
    Pipeline->EngineContext = newContext;
    newContext = NULL;

cleanup:
    if (FAILED(hr))
    {
        // If a new context has been created, release any memory 
        // pointed to by various data members in the context and 
        // then release the context. The following example assumes 
        // that your adapter contains a handle
        // for a hash object and a pointer to another object.
        if (newContext != NULL)
        {
            // Close any open CNG handles and release the hash object memory.
            _AdapterCleanupCrypto(newContext);

            // Release any other object pointed to by the context.
            if (newContext->SomePointerField != NULL)
            {
                _AdapterRelease(newContext->SomePointerField);
            }

            // Release the context
            _AdapterRelease(newContext);
        }
    }
    return hr;

}

```





## -see-also




<a href="https://msdn.microsoft.com/a4bc8ef1-6005-4661-9bb1-20ea08d9a125">EngineAdapterDetach</a>



<a href="https://msdn.microsoft.com/5f04d912-f9bc-41d4-aa9e-b843e4b5a994">Plug-in Functions</a>



<a href="https://msdn.microsoft.com/91243128-0543-4df9-bde8-74ef5ae46914">SensorAdapterAttach</a>



<a href="https://msdn.microsoft.com/6abded6b-12e0-4cc6-a011-0b18e8ea747b">StorageAdapterAttach</a>



<a href="https://msdn.microsoft.com/b5fc2b14-b0b6-4327-a42a-ecae41c3e12a">WINBIO_PIPELINE</a>
 

 

