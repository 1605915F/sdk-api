---
UID: NF:iphlpapi.DeleteIPAddress
title: DeleteIPAddress function
author: windows-sdk-content
description: The DeleteIPAddress function deletes an IP address previously added using AddIPAddress.
old-location: iphlp\deleteipaddress.htm
tech.root: IpHlp
ms.assetid: d7ed986d-d62e-4723-ab74-85c3edfdf4ff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DeleteIPAddress, DeleteIPAddress function [IP Helper], _iphlp_deleteipaddress, iphlp.deleteipaddress, iphlpapi/DeleteIPAddress
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - DeleteIPAddress
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DeleteIPAddress function


## -description


The 
<b>DeleteIPAddress</b> function deletes an IP address previously added using 
<a href="https://msdn.microsoft.com/669264cd-a43c-4681-9416-2704d4232685">AddIPAddress</a>.


## -parameters




### -param NTEContext [in]

The Net Table Entry (NTE) context for the IP address. This context was returned by the previous call to 
<a href="https://msdn.microsoft.com/669264cd-a43c-4681-9416-2704d4232685">AddIPAddress</a>.


## -returns



The function returns <b>NO_ERROR</b> (zero) if the function is successful. 

If the function fails, the return value is one of the following error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
Access is denied. This error is returned on Windows Vista and Windows Server 2008 under several conditions that include the following: the  user lacks the required administrative privileges on the local computer or the application is not running in an enhanced shell as the built-in Administrator (RunAs administrator).  

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
An input parameter is invalid, no action was taken.  

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The IPv4 transport is not configured on the local computer.

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
<a href="https://msdn.microsoft.com/b9d61342-4bcf-42e9-96f1-a5993dfb6c0c">FormatMessage</a> to obtain the message string for the returned error.

</td>
</tr>
</table>
 




## -remarks



On Windows Vista and later, the <b>DeleteIPAddress</b> function can only be called by a user logged on as a member of the Administrators group. If <b>DeleteIPAddress</b> is called by a user that is not a member of the Administrators group, the function call will fail and <b>ERROR_ACCESS_DENIED</b> is returned. This function can also fail because of user account control (UAC) on Windows Vista and later. If an application that contains this function is executed by a user logged on as a member of the Administrators group other than the built-in Administrator, this call will fail unless the application has been marked in the manifest file with a <b>requestedExecutionLevel</b> set to requireAdministrator. If the application on Windows Vista and later lacks this manifest file, a user logged on as a member of the Administrators group other than the built-in Administrator must then be executing the application in an enhanced shell as the built-in Administrator (RunAs administrator) for this function to succeed.



<div class="alert"><b>Note</b>  On Windows NT 4.0 and Windows 2000 and later, this function executes a privileged operation. For this function to execute successfully, the caller must be logged on as a member of the Administrators group or the NetworkConfigurationOperators group.</div>
<div> </div>

#### Examples

The following example retrieves the IP address table, then adds the IP address 192.168.0.27 to the first adapter. The IP address that was added is then deleted.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#ifndef WIN32_LEAN_AND_MEAN
#define WIN32_LEAN_AND_MEAN
#endif

#include &lt;windows.h&gt;
#include &lt;winsock2.h&gt;
#include &lt;iphlpapi.h&gt;
#include &lt;stdio.h&gt;
#include &lt;stdlib.h&gt;

#pragma comment(lib, "iphlpapi.lib")
#pragma comment(lib, "ws2_32.lib")

int main()
{
    // Declare and initialize variables
    PMIB_IPADDRTABLE pIPAddrTable;
    DWORD dwSize = 0;
    DWORD dwRetVal;

    // IP and mask we will be adding
    UINT iaIPAddress;
    UINT imIPMask;

    // Variables where handles to the added IP will be returned
    ULONG NTEContext = 0;
    ULONG NTEInstance = 0;

    LPVOID lpMsgBuf;


    // Before calling AddIPAddress we use GetIpAddrTable to get
    // an adapter to which we can add the IP.
    pIPAddrTable = (MIB_IPADDRTABLE *) malloc(sizeof (MIB_IPADDRTABLE));

    // Make an initial call to GetIpAddrTable to get the
    // necessary size into the dwSize variable
    if (GetIpAddrTable(pIPAddrTable, &amp;dwSize, 0) == ERROR_INSUFFICIENT_BUFFER) {
        GlobalFree(pIPAddrTable);
        pIPAddrTable = (MIB_IPADDRTABLE *) malloc(dwSize);
    }
    // Make a second call to GetIpAddrTable to get the
    // actual data we want
    if ((dwRetVal = GetIpAddrTable(pIPAddrTable, &amp;dwSize, 0)) == NO_ERROR) {
        printf("\tAddress: %ld\n", pIPAddrTable-&gt;table[0].dwAddr);
        printf("\tMask:    %ld\n", pIPAddrTable-&gt;table[0].dwMask);
        printf("\tIndex:   %ld\n", pIPAddrTable-&gt;table[0].dwIndex);
        printf("\tBCast:   %ld\n", pIPAddrTable-&gt;table[0].dwBCastAddr);
        printf("\tReasm:   %ld\n", pIPAddrTable-&gt;table[0].dwReasmSize);
    } else {
        printf("Call to GetIpAddrTable failed.\n");
    }

    // IP and mask we will be adding

    iaIPAddress = inet_addr("192.168.0.27");
    imIPMask = inet_addr("255.255.255.0");

    if ((dwRetVal = AddIPAddress(iaIPAddress,
                                 imIPMask,
                                 pIPAddrTable-&gt;table[0].dwIndex,
                                 &amp;NTEContext, &amp;NTEInstance)) == NO_ERROR) {
        printf("\tIP address added.\n");
    }

    else {
        printf("Error adding IP address.\n");

        if (FormatMessage(FORMAT_MESSAGE_ALLOCATE_BUFFER | FORMAT_MESSAGE_FROM_SYSTEM | FORMAT_MESSAGE_IGNORE_INSERTS, NULL, dwRetVal, MAKELANGID(LANG_NEUTRAL, SUBLANG_DEFAULT),       // Default language
                          (LPTSTR) &amp; lpMsgBuf, 0, NULL)) {
            printf("\tError: %s", lpMsgBuf);
        }
        LocalFree(lpMsgBuf);
    }

    // Delete the IP we just added using the NTEContext
    // variable where the handle was returned       
    if ((dwRetVal = DeleteIPAddress(NTEContext)) == NO_ERROR) {
        printf("\tIP Address Deleted.\n");
    } else {
        printf("\tCall to DeleteIPAddress failed.\n");
    }

    exit(0);
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/669264cd-a43c-4681-9416-2704d4232685">AddIPAddress</a>



<a href="https://msdn.microsoft.com/2de88e92-5fa5-4d8d-9448-67a33bf02f05">IP Helper Function Reference</a>



<a href="https://msdn.microsoft.com/4896a9f8-0486-4380-bf49-d1c9ef114acc">IP Helper Start Page</a>
 

 

