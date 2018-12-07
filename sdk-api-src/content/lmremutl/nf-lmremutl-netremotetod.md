---
UID: NF:lmremutl.NetRemoteTOD
title: NetRemoteTOD function
author: windows-sdk-content
description: The NetRemoteTOD function returns the time of day information from a specified server.
old-location: netmgmt\netremotetod.htm
tech.root: netmgmt
ms.assetid: 5a935e09-f188-4ee1-b998-c67488475baa
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: NetRemoteTOD, NetRemoteTOD function [Network Management], _win32_netremotetod, lmremutl/NetRemoteTOD, netmgmt.netremotetod
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: lmremutl.h
req.include-header: Lm.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Netapi32.lib
req.dll: Netapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Netapi32.dll
api_name:
 - NetRemoteTOD
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# NetRemoteTOD function


## -description


The
				<b>NetRemoteTOD</b> function returns the time of day information from a specified server.


## -parameters




### -param UncServerName [in]

Pointer to a constant string that specifies the DNS or NetBIOS name of the remote server on which the function is to execute. If this parameter is <b>NULL</b>, the local computer is used.


### -param BufferPtr [out]

Pointer to the address that receives the 
<a href="https://msdn.microsoft.com/bf89f071-5c04-40c2-a7b7-4e59fc9eaa02">TIME_OF_DAY_INFO</a> information structure. This buffer is allocated by the system and must be freed using the 
<a href="https://msdn.microsoft.com/0e99483c-8cd7-402a-8bf6-1e0118764dd3">NetApiBufferFree</a> function.


## -returns



If the function succeeds, the return value is NERR_Success.

If the function fails, the return value is a system error code. For a list of error codes, see 
<a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">System Error Codes</a>.




## -remarks



No special group membership is required to successfully execute the 
<b>NetRemoteTOD</b> function.


#### Examples

The following code sample demonstrates how to retrieve and print the current date and time with a call to the 
<b>NetRemoteTOD</b> function. To do this, the sample uses the 
<a href="https://msdn.microsoft.com/bf89f071-5c04-40c2-a7b7-4e59fc9eaa02">TIME_OF_DAY_INFO</a> structure. Finally, the sample frees the memory allocated for the information buffer.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#include &lt;stdio.h&gt;
#include &lt;windows.h&gt; 
#include &lt;lm.h&gt;
#pragma comment(lib, "netapi32.lib")

#ifndef UNICODE
#define UNICODE
#endif

int wmain(int argc, wchar_t *argv[])
{
   LPTIME_OF_DAY_INFO pBuf = NULL;
   NET_API_STATUS nStatus;
   LPTSTR pszServerName = NULL;

   if (argc &gt; 2)
   {
      fwprintf(stderr, L"Usage: %s [\\\\ServerName]\n", argv[0]);
      exit(1);
   }
   // The server is not the default local computer.
   //
   if (argc == 2)
      pszServerName = (LPTSTR) argv[1];
   //
   // Call the NetRemoteTOD function.
   //
   nStatus = NetRemoteTOD((LPCWSTR) pszServerName,
                          (LPBYTE *)&amp;pBuf);
   //
   // If the function succeeds, display the current date and time.
   //
   if (nStatus == NERR_Success)
   {
      if (pBuf != NULL)
      {
         fprintf(stderr, "\nThe current date is: %d/%d/%d\n",
                 pBuf-&gt;tod_month, pBuf-&gt;tod_day, pBuf-&gt;tod_year);
         fprintf(stderr, "The current time is: %d:%d:%d\n",
                 pBuf-&gt;tod_hours, pBuf-&gt;tod_mins, pBuf-&gt;tod_secs);
      }
   }
   //
   // Otherwise, display a system error.
   else
      fprintf(stderr, "A system error has occurred: %d\n", nStatus);
   //
   // Free the allocated buffer.
   //
   if (pBuf != NULL)
      NetApiBufferFree(pBuf);

   return 0;
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/dd159e2e-f37e-46b2-b980-008b73d40b39">Network
		  Management Functions</a>



<a href="https://msdn.microsoft.com/426c7b2e-027c-4a88-97b7-eba5201d0f0d">Network Management
		  Overview</a>



<a href="https://msdn.microsoft.com/e925d6d1-9347-4074-a12e-175b2115e71e">Remote
		  Utility Functions</a>



<a href="https://msdn.microsoft.com/bf89f071-5c04-40c2-a7b7-4e59fc9eaa02">TIME_OF_DAY_INFO</a>
 

 

