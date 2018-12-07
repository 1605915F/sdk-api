---
UID: NC:winbio_adapter.PIBIO_STORAGE_GET_CURRENT_RECORD_FN
title: PIBIO_STORAGE_GET_CURRENT_RECORD_FN
author: windows-sdk-content
description: Retrieves the contents of the current record in the pipeline result set.
old-location: secbiomet\storageadaptergetcurrentrecord.htm
tech.root: SecBioMet
ms.assetid: a06550da-c6ea-44e5-b54f-8005bcbc0364
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PIBIO_STORAGE_GET_CURRENT_RECORD_FN, PIBIO_STORAGE_GET_CURRENT_RECORD_FN callback, StorageAdapterGetCurrentRecord, StorageAdapterGetCurrentRecord callback function [Windows Biometric Framework API], secbiomet.storageadaptergetcurrentrecord, winbio_adapter/StorageAdapterGetCurrentRecord
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
 - StorageAdapterGetCurrentRecord
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PIBIO_STORAGE_GET_CURRENT_RECORD_FN callback function


## -description


Called by the Windows Biometric Framework or by an engine adapter to retrieve the contents of the current record in the pipeline result set.


## -parameters




### -param Pipeline [in, out]

Pointer to the <a href="https://msdn.microsoft.com/b5fc2b14-b0b6-4327-a42a-ecae41c3e12a">WINBIO_PIPELINE</a> structure associated with the biometric unit performing the operation.


### -param RecordContents [out]

Pointer to a <a href="https://msdn.microsoft.com/fd638a08-cff0-4984-8580-a1eecd509a1f">WINBIO_STORAGE_RECORD</a> structure that will receive the contents of the record.


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
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Memory could not be allocated for the record.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
A mandatory pointer argument is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>WINBIO_E_DATABASE_NO_RESULTS</b></b></dt>
</dl>
</td>
<td width="60%">
There are no records in the result set.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WINBIO_E_INVALID_DEVICE_STATE</b></dt>
</dl>
</td>
<td width="60%">
The <b>StorageContext</b> member of the pipeline object is <b>NULL</b> or the <b>FileHandle</b> member is not valid.

</td>
</tr>
</table>
 




## -remarks



Any addresses returned by this function in the WINBIO_STORAGE_RECORD structure must remain valid until one of the following functions is called:


<ul>
<li>
<a href="https://msdn.microsoft.com/736688c3-2c2c-4244-9f49-98ad0fe2d141">StorageAdapterFirstRecord</a>
</li>
<li>
<a href="https://msdn.microsoft.com/e0025167-0778-474e-baca-ffc767822893">StorageAdapterNextRecord</a>
</li>
<li>
<a href="https://msdn.microsoft.com/773aacd1-a34a-4c5a-b615-2a5485f13ca1">StorageAdapterQueryByContent</a>
</li>
<li>
<a href="https://msdn.microsoft.com/b2c93122-fae1-44ad-97d4-f90115194a31">StorageAdapterQueryBySubject</a>
</li>
<li>
<a href="https://msdn.microsoft.com/d7022363-01e9-4675-9bd0-e9369d237c3c">StorageAdapterClearContext</a>
</li>
</ul>
Calling the <i>StorageAdapterGetCurrentRecord</i> function does not change the result set pointer. If the pointer is already on the last record in the set, repeatedly calling this function will return the same record contents and an <b>HRESULT</b> value of S_OK.


#### Examples

The following pseudocode shows one possible implementation of this function. The example does not compile. You must adapt it to suit your purpose.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>/////////////////////////////////////////////////////////////////////////////////////////
//
// StorageAdapterGetCurrentRecord
//
// Purpose:
//      Retrieves the contents of the current record in the pipeline result set.
//
// Parameters:
//      Pipeline       - Pointer to a WINBIO_PIPELINE structure associated with 
//                       the biometric unit performing the operation.
//      RecordContents - Pointer to a WINBIO_STORAGE_RECORD structure that will receive 
//                       the contents of the record.
//
static HRESULT
WINAPI
StorageAdapterGetCurrentRecord(
    __inout PWINBIO_PIPELINE Pipeline,
    __out PWINBIO_STORAGE_RECORD RecordContents
    )
{
    HRESULT hr = S_OK;
    struct _MY_ADAPTER_RECORD_HEADER *recordHeader = NULL;
    LARGE_INTEGER dataOffset = {0};
    SIZE_T allocationSize = 0;

    // Verify that pointer arguments are not NULL.
    if (!ARGUMENT_PRESENT(Pipeline) ||
        !ARGUMENT_PRESENT(RecordContents))
    {
        hr = E_POINTER;
        goto cleanup;
    }

    // Retrieve the context from the pipeline.
    PWINBIO_STORAGE_CONTEXT storageContext = (PWINBIO_STORAGE_CONTEXT)Pipeline-&gt;StorageContext;

    // Verify the pipeline state.
    if (storageContext == NULL || storageContext-&gt;FileHandle == INVALID_HANDLE_VALUE)
    {
        hr =  WINBIO_E_INVALID_DEVICE_STATE;
        goto cleanup;
    }

    // Call a custom function (_ResultSetGetCurrent) to retrieve the header
    // contents of the current record in the result set. This function should
    // also return the file offset of the template data in the record.
    hr = _ResultSetGetCurrent(
            &amp;storageContext-&gt;ResultSet,
            &amp;recordHeader,
            &amp;dataOffset
            );
    if (FAILED(hr))
    {
        goto cleanup;
    }

    RecordContents-&gt;Identity = &amp;recordHeader-&gt;Identity;
    RecordContents-&gt;SubFactor = recordHeader-&gt;SubFactor;
    RecordContents-&gt;IndexVector = _GetIndexVector(recordHeader);
    RecordContents-&gt;IndexElementCount = recordHeader-&gt;IndexElementCount;

    // Release any template data buffers created by previous calls to the
    // StorageAdapterGetCurrentRecord function. 
    if (storageContext-&gt;RawRecordData != NULL)
    {
        _AdapterRelease(storageContext-&gt;RawRecordData);
        storageContext-&gt;RawRecordData = NULL;
        storageContext-&gt;PayloadBlob = NULL;
    }

    if (storageContext-&gt;DecryptedTemplate != NULL)
    {
        // You must call SecureZeroMemory to clear any memory that contains
        // a plaintext version of the template data.
        SecureZeroMemory(
            storageContext-&gt;DecryptedTemplate, 
            storageContext-&gt;DecryptedTemplateSize
            );
        _AdapterRelease(storageContext-&gt;DecryptedTemplate);
        storageContext-&gt;DecryptedTemplate = NULL;
        storageContext-&gt;DecryptedTemplateSize = 0;
    }

    // Allocate a buffer for the template and payload portions of the record.
    allocationSize = 
        recordHeader-&gt;EncryptedTemplateBlobSize + 
        recordHeader-&gt;PayloadBlobSize;

    storageContext-&gt;RawRecordData = (PUCHAR)_AdapterAlloc(allocationSize);
    if (storageContext-&gt;RawRecordData == NULL)
    {
        hr = E_OUTOFMEMORY;
        goto cleanup;
    }

    // Call a custom function (_ReadRecordData) that reads the non-header
    // portion of the record.
    hr = _ReadRecordData(
            Pipeline-&gt;StorageHandle,
            dataOffset,
            storageContext-&gt;RawRecordData,
            (DWORD)allocationSize,
            (PDWORD)&amp;storageContext-&gt;RawRecordDataSize
            );
    if (FAILED(hr))
    {
        goto cleanup;
    }

    // Call a custom function (_DecryptTemplate) that decrypts the template 
    // data and stores a pointer to the plaintext version in the storage context.
    hr = _DecryptTemplate(
            &amp;storageContext-&gt;CryptoContext,
            storageContext-&gt;RawRecordData,
            recordHeader-&gt;EncryptedTemplateBlobSize,
            &amp;storageContext-&gt;DecryptedTemplate,
            &amp;storageContext-&gt;DecryptedTemplateSize
            );
    if (FAILED(hr))
    {
        goto cleanup;
    }

    // Set up return values for the caller. These values will remain valid until
    // the next query or get operation.
    RecordContents-&gt;TemplateBlob = storageContext-&gt;DecryptedTemplate;
    RecordContents-&gt;TemplateBlobSize = recordHeader-&gt;TemplateBlobSize;

    if (recordHeader-&gt;PayloadBlobSize != 0)
    {
        RecordContents-&gt;PayloadBlob = 
            storageContext-&gt;RawRecordData + 
            recordHeader-&gt;EncryptedTemplateBlobSize;

        RecordContents-&gt;PayloadBlobSize = recordHeader-&gt;PayloadBlobSize;
    }
    else
    {
        RecordContents-&gt;PayloadBlob = NULL;
        RecordContents-&gt;PayloadBlobSize = 0;
    }

cleanup:

    if (FAILED(hr))
    {
        if (storageContext-&gt;RawRecordData != NULL)
        {
            // Because the raw record data (including the payload blob) is
            // encrypted, it is not necessary to call SecureZeroMemory.
            _AdapterRelease(storageContext-&gt;RawRecordData);
            storageContext-&gt;RawRecordData = NULL;
            storageContext-&gt;PayloadBlob = NULL;
        }
        if (storageContext-&gt;DecryptedTemplate != NULL)
        {
            // You must call SecureZeroMemory to clear the plaintext version 
            // of the template before releasing it.
            SecureZeroMemory(
                storageContext-&gt;DecryptedTemplate, 
                storageContext-&gt;DecryptedTemplateSize
                );
            _AdapterRelease(storageContext-&gt;DecryptedTemplate);
            storageContext-&gt;DecryptedTemplate = NULL;
            storageContext-&gt;DecryptedTemplateSize = 0;
        }
    }

    return hr;
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/5f04d912-f9bc-41d4-aa9e-b843e4b5a994">Plug-in Functions</a>
 

 

