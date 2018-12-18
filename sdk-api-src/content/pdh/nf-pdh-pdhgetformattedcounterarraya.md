---
UID: NF:pdh.PdhGetFormattedCounterArrayA
title: PdhGetFormattedCounterArrayA function
author: windows-sdk-content
description: Returns an array of formatted counter values. Use this function when you want to format the counter values of a counter that contains a wildcard character for the instance name.
old-location: perf\pdhgetformattedcounterarray.htm
tech.root: perfctrs
ms.assetid: 0f388c7e-d0c8-461d-908c-48af92166996
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PDH_FMT_1000, PDH_FMT_DOUBLE, PDH_FMT_LARGE, PDH_FMT_LONG, PDH_FMT_NOCAP100, PDH_FMT_NOSCALE, PdhGetFormattedCounterArray, PdhGetFormattedCounterArray function [Perf], PdhGetFormattedCounterArrayA, PdhGetFormattedCounterArrayW, _win32_pdhgetformattedcounterarray, base.pdhgetformattedcounterarray, pdh/PdhGetFormattedCounterArray, pdh/PdhGetFormattedCounterArrayA, pdh/PdhGetFormattedCounterArrayW, perf.pdhgetformattedcounterarray
ms.topic: function
req.header: pdh.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: PdhGetFormattedCounterArrayW (Unicode) and PdhGetFormattedCounterArrayA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Pdh.lib
req.dll: Pdh.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Pdh.dll
api_name:
 - PdhGetFormattedCounterArray
 - PdhGetFormattedCounterArrayA
 - PdhGetFormattedCounterArrayW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PdhGetFormattedCounterArrayA function


## -description


Returns an array of formatted counter values. Use this function when you want to format the counter values of a counter that contains a wildcard character for the instance name.
		


## -parameters




### -param hCounter [in]

Handle to the counter whose current value you want to format. The 
<a href="https://msdn.microsoft.com/b8b9a332-ce28-46d4-92e2-91f9f6c24da5">PdhAddCounter</a> function returns this handle.


### -param dwFormat [in]

Determines the data type of the formatted value. Specify one of the following values. 



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="PDH_FMT_DOUBLE"></a><a id="pdh_fmt_double"></a><dl>
<dt><b>PDH_FMT_DOUBLE</b></dt>
</dl>
</td>
<td width="60%">
Return data as a double-precision floating point real.

</td>
</tr>
<tr>
<td width="40%"><a id="PDH_FMT_LARGE"></a><a id="pdh_fmt_large"></a><dl>
<dt><b>PDH_FMT_LARGE</b></dt>
</dl>
</td>
<td width="60%">
Return data as a 64-bit integer.

</td>
</tr>
<tr>
<td width="40%"><a id="PDH_FMT_LONG"></a><a id="pdh_fmt_long"></a><dl>
<dt><b>PDH_FMT_LONG</b></dt>
</dl>
</td>
<td width="60%">
Return data as a long integer.

</td>
</tr>
</table>
 

You can use the bitwise inclusive OR operator (|) to combine the data type with one of the following scaling factors.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="PDH_FMT_NOSCALE"></a><a id="pdh_fmt_noscale"></a><dl>
<dt><b>PDH_FMT_NOSCALE</b></dt>
</dl>
</td>
<td width="60%">
Do not apply the counter's default scaling factor.

</td>
</tr>
<tr>
<td width="40%"><a id="PDH_FMT_NOCAP100"></a><a id="pdh_fmt_nocap100"></a><dl>
<dt><b>PDH_FMT_NOCAP100</b></dt>
</dl>
</td>
<td width="60%">
Counter values greater than 100 (for example, counter values measuring the processor load on multiprocessor computers) will not be reset to 100. The default behavior is that counter values are capped at a value of 100.

</td>
</tr>
<tr>
<td width="40%"><a id="PDH_FMT_1000"></a><a id="pdh_fmt_1000"></a><dl>
<dt><b>PDH_FMT_1000</b></dt>
</dl>
</td>
<td width="60%">
Multiply the actual value by 1,000.

</td>
</tr>
</table>
 


### -param lpdwBufferSize [in, out]

Size of the <i>ItemBuffer</i> buffer, in bytes. If zero on input, the function returns PDH_MORE_DATA and sets this parameter to the required buffer size. If the buffer is larger than the required size, the function sets this parameter to the actual size of the buffer that was used. If the specified size on input is greater than zero but less than the required size, you should not rely on the returned size to reallocate the buffer.


### -param lpdwItemCount [out]

Number of counter values in the <i>ItemBuffer</i> buffer.


### -param ItemBuffer [out]

Caller-allocated buffer that receives an array of 
<a href="https://msdn.microsoft.com/d3bc6ad3-0cab-4843-ae1d-5f384948a1ea">PDH_FMT_COUNTERVALUE_ITEM</a> structures; the structures contain the counter values. Set to <b>NULL</b> if <i>lpdwBufferSize</i> is zero.


## -returns



If the function succeeds, it returns ERROR_SUCCESS.
						

If the function fails, the return value is a 
<a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a> or a 
<a href="https://msdn.microsoft.com/ea67d798-81db-44ad-b0fb-24e0c3be7388">PDH error code</a>. The following are possible values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PDH_MORE_DATA</b></dt>
</dl>
</td>
<td width="60%">
The <i>ItemBuffer</i> buffer is not large enough to contain the object name. This return value is expected if <i>lpdwBufferSize</i> is zero on input. If the specified size on input is greater than zero but less than the required size, you should not rely on the returned size to reallocate the buffer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PDH_INVALID_ARGUMENT</b></dt>
</dl>
</td>
<td width="60%">
A parameter is not valid or is incorrectly formatted. For example, on some releases you could receive this error if the specified size on input is greater than zero but less than the required size.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PDH_INVALID_HANDLE</b></dt>
</dl>
</td>
<td width="60%">
The counter handle is not valid.

</td>
</tr>
</table>
 




## -remarks



You should call this function twice, the first time to get the required buffer size (set <i>ItemBuffer</i> to <b>NULL</b> and <i>lpdwBufferSize</i> to 0), and the second time to get the data.

The data for the counter is locked for the duration of the call to 
<b>PdhGetFormattedCounterArray</b> to prevent any changes during the processing of the call.


#### Examples

The following example shows how to use this function.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>
#include &lt;windows.h&gt;
#include &lt;stdio.h&gt;
#include &lt;pdh.h&gt;
#include &lt;pdhmsg.h&gt;

#pragma comment(lib, "pdh.lib")

CONST PWSTR COUNTER_PATH = L"\\Processor(*)\\% Processor Time";
CONST ULONG SAMPLE_INTERVAL_MS = 1000;

void main()
{
    PDH_HQUERY hQuery = NULL;
    PDH_STATUS status = ERROR_SUCCESS;
    PDH_HCOUNTER hCounter = NULL;   
    DWORD dwBufferSize = 0;         // Size of the pItems buffer
    DWORD dwItemCount = 0;          // Number of items in the pItems buffer
    PDH_FMT_COUNTERVALUE_ITEM *pItems = NULL;  // Array of PDH_FMT_COUNTERVALUE_ITEM structures

    if (status = PdhOpenQuery(NULL, 0, &amp;hQuery))
    {
        wprintf(L"PdhOpenQuery failed with 0x%x.\n", status);
        goto cleanup;
    }

    // Specify a counter object with a wildcard for the instance.
    if (status = PdhAddCounter(hQuery, COUNTER_PATH, 0, &amp;hCounter))
    {
        wprintf(L"PdhAddCounter failed with 0x%x.\n", status);
        goto cleanup;
    }

    // Some counters need two sample in order to format a value, so
    // make this call to get the first value before entering the loop.
    if (status = PdhCollectQueryData(hQuery))
    {
        wprintf(L"PdhCollectQueryData failed with 0x%x.\n", status);
        goto cleanup;
    }

    for (int i = 0; i &lt; 10; i++)
    {
        Sleep(SAMPLE_INTERVAL_MS);

        if (status = PdhCollectQueryData(hQuery))
        {
            wprintf(L"PdhCollectQueryData failed with 0x%x.\n", status);
            goto cleanup;
        }

        // Get the required size of the pItems buffer.
        status = PdhGetFormattedCounterArray(hCounter, PDH_FMT_DOUBLE, &amp;dwBufferSize, &amp;dwItemCount, pItems);
        if (PDH_MORE_DATA == status)
        {
            pItems = (PDH_FMT_COUNTERVALUE_ITEM *) malloc(dwBufferSize);
            if (pItems)
            {
                status = PdhGetFormattedCounterArray(hCounter, PDH_FMT_DOUBLE, &amp;dwBufferSize, &amp;dwItemCount, pItems);
                if (ERROR_SUCCESS == status)
                {
                    // Loop through the array and print the instance name and counter value.
                    for (DWORD i = 0; i &lt; dwItemCount; i++)
                    {
                        wprintf(L"counter: %s, value %.20g\n", pItems[i].szName, pItems[i].FmtValue.doubleValue);
                    }
                }
                else
                {
                    wprintf(L"Second PdhGetFormattedCounterArray call failed with 0x%x.\n", status);
                    goto cleanup;
                }

                free(pItems);
                pItems = NULL;
                dwBufferSize = dwItemCount = 0;
            }
            else
            {
                wprintf(L"malloc for PdhGetFormattedCounterArray failed.\n");
                goto cleanup;
            }
        }
        else
        {
            wprintf(L"PdhGetFormattedCounterArray failed with 0x%x.\n", status);
            goto cleanup;
        }
    }

cleanup:

    if (pItems)
        free(pItems);

    if (hQuery)
        PdhCloseQuery(hQuery); // Closes all counter handles and the query handle
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/d3bc6ad3-0cab-4843-ae1d-5f384948a1ea">PDH_FMT_COUNTERVALUE_ITEM</a>



<a href="https://msdn.microsoft.com/b8b9a332-ce28-46d4-92e2-91f9f6c24da5">PdhAddCounter</a>



<a href="https://msdn.microsoft.com/cd104b26-1498-4f95-a411-97d868b43836">PdhGetFormattedCounterValue</a>



<a href="https://msdn.microsoft.com/03b30d08-6901-45cd-bd6d-d2672eb0f914">PdhGetRawCounterArray</a>



<a href="https://msdn.microsoft.com/bb246c82-8748-4e2f-9f44-a206199aff90">PdhGetRawCounterValue</a>
 

 

