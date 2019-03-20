---
UID: NF:iphlpapi.GetTcpStatistics
title: GetTcpStatistics function (iphlpapi.h)
author: windows-sdk-content
description: The GetTcpStatistics function retrieves the TCP statistics for the local computer.
old-location: iphlp\gettcpstatistics.htm
tech.root: IpHlp
ms.assetid: 841cdeaa-6284-4b39-a218-69937eca1982
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetTcpStatistics, GetTcpStatistics function [IP Helper], _iphlp_gettcpstatistics, iphlp.gettcpstatistics, iphlpapi/GetTcpStatistics
ms.topic: function
req.header: iphlpapi.h
req.include-header: 
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
req.lib: Iphlpapi.lib
req.dll: Iphlpapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Iphlpapi.dll
api_name:
 - GetTcpStatistics
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetTcpStatistics function


## -description


The 
<b>GetTcpStatistics</b> function retrieves the TCP statistics for the local computer.


## -parameters




### -param Statistics [out]

A pointer to a 
<a href="https://msdn.microsoft.com/08d85d02-62a0-479d-bf56-5dad452436f3">MIB_TCPSTATS</a> structure that receives the TCP statistics for the local computer.


## -returns



If the function succeeds, the return value is NO_ERROR.

If the function fails, the return value is one of the following error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The <i>pStats</i> parameter is <b>NULL</b>, or 
<a href="https://msdn.microsoft.com/841cdeaa-6284-4b39-a218-69937eca1982">GetTcpStatistics</a> is unable to write to the memory pointed to by the <i>pStats</i> parameter.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Other</b></dt>
</dl>
</td>
<td width="60%">
Use 
the <a href="https://msdn.microsoft.com/b9d61342-4bcf-42e9-96f1-a5993dfb6c0c">FormatMessage</a> function to obtain the message string for the returned error.

</td>
</tr>
</table>
 




## -remarks



The 
<b>GetTcpStatistics</b> function returns the TCP statistics for IPv4 on the current computer.     On Windows XP and later, the <a href="https://msdn.microsoft.com/78cfc69d-eae8-49c1-a460-6527a61f773d">GetTcpStatisticsEx</a> can be used to obtain the TCP statistics for either IPv4 or IPv6.


#### Examples

The following example retrieves the TCP statistics for the local computer and prints some values from the returned data.


```cpp
//#include <windows.h>
#include <winsock2.h>
#include <ws2tcpip.h>
#include <iphlpapi.h>
#include <stdio.h>

#pragma comment(lib, "iphlpapi.lib")

#define MALLOC(x) HeapAlloc(GetProcessHeap(), 0, (x)) 
#define FREE(x) HeapFree(GetProcessHeap(), 0, (x))

/* Note: could also use malloc() and free() */

int main()
{
    PMIB_TCPSTATS pTCPStats;
    DWORD dwRetVal = 0;

    pTCPStats = (MIB_TCPSTATS*) MALLOC (sizeof(MIB_TCPSTATS));
    if (pTCPStats == NULL) {
        printf("Error allocating memory\n");
        return 1;
    }

    if ((dwRetVal = GetTcpStatistics(pTCPStats)) == NO_ERROR) {
      printf("\tActive Opens: %ld\n", pTCPStats->dwActiveOpens);
      printf("\tPassive Opens: %ld\n", pTCPStats->dwPassiveOpens);
      printf("\tSegments Recv: %ld\n", pTCPStats->dwInSegs);
      printf("\tSegments Xmit: %ld\n", pTCPStats->dwOutSegs);
      printf("\tTotal # Conxs: %ld\n", pTCPStats->dwNumConns);
    }
    else {
      printf("GetTcpStatistics failed with error: %ld\n", dwRetVal);
      
      LPVOID lpMsgBuf;
      if (FormatMessage( FORMAT_MESSAGE_ALLOCATE_BUFFER | 
        FORMAT_MESSAGE_FROM_SYSTEM | 
        FORMAT_MESSAGE_IGNORE_INSERTS,
        NULL,
        dwRetVal,
        MAKELANGID(LANG_NEUTRAL, SUBLANG_DEFAULT), // Default language
        (LPTSTR) &lpMsgBuf,
        0,
        NULL )) {
        printf("\tError: %s", lpMsgBuf);
      }
      LocalFree( lpMsgBuf );
    }

    if (pTCPStats)
        FREE (pTCPStats);
}

```





## -see-also




<a href="https://msdn.microsoft.com/b10ec58b-54fe-4068-beb9-6909ad7cecf7">GetIcmpStatistics</a>



<a href="https://msdn.microsoft.com/15daaa34-2011-462a-9543-f8d7ccb9f6fd">GetIpStatistics</a>



<a href="https://msdn.microsoft.com/78cfc69d-eae8-49c1-a460-6527a61f773d">GetTcpStatisticsEx</a>



<a href="https://msdn.microsoft.com/a86e5758-a984-4483-8e9c-c482a7676a20">GetUdpStatistics</a>



<a href="https://msdn.microsoft.com/2de88e92-5fa5-4d8d-9448-67a33bf02f05">IP Helper Function Reference</a>



<a href="https://msdn.microsoft.com/4896a9f8-0486-4380-bf49-d1c9ef114acc">IP Helper Start Page</a>



<a href="https://msdn.microsoft.com/08d85d02-62a0-479d-bf56-5dad452436f3">MIB_TCPSTATS</a>
 

 

