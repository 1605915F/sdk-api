---
UID: NS:tcpmib._MIB_TCPTABLE_OWNER_PID
title: MIB_TCPTABLE_OWNER_PID
author: windows-sdk-content
description: Contains a table of process IDs (PIDs) and the IPv4 TCP links that are context bound to these PIDs.
old-location: mib\mib_tcptable_owner_pid.htm
tech.root: MIB
ms.assetid: ef39b832-1f22-468a-8734-c7d9bd3ac965
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMIB_TCPTABLE_OWNER_PID, MIB_TCPTABLE_OWNER_PID, MIB_TCPTABLE_OWNER_PID structure [MIB], PMIB_TCPTABLE_OWNER_PID, PMIB_TCPTABLE_OWNER_PID structure pointer [MIB], iprtrmib/MIB_TCPTABLE_OWNER_PID, iprtrmib/PMIB_TCPTABLE_OWNER_PID, mib.mib_tcptable_owner_pid, tcpmib/MIB_TCPTABLE_OWNER_PID, tcpmib/PMIB_TCPTABLE_OWNER_PID"
ms.topic: struct
req.header: tcpmib.h
req.include-header: Iphlpapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2008, Windows Server 2003 with SP1 [desktop apps only]
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
 - HeaderDef
api_location:
 - Tcpmib.h
 - Iprtrmib.h
api_name:
 - MIB_TCPTABLE_OWNER_PID
product: Windows
targetos: Windows
req.typenames: MIB_TCPTABLE_OWNER_PID, *PMIB_TCPTABLE_OWNER_PID
req.redist: 
---

# MIB_TCPTABLE_OWNER_PID structure


## -description


The <b>MIB_TCPTABLE_OWNER_PID</b> structure contains a table of process IDs (PIDs)  and the IPv4 TCP links that  are context bound to these PIDs.


## -struct-fields




### -field dwNumEntries

The number of <a href="https://msdn.microsoft.com/220b69a4-b372-4eff-8d5a-eca0d39b8af9">MIB_TCPROW_OWNER_PID</a> elements in the <b>table</b>.


### -field table

Array of <a href="https://msdn.microsoft.com/220b69a4-b372-4eff-8d5a-eca0d39b8af9">MIB_TCPROW_OWNER_PID</a> structures returned by a call to <a href="https://msdn.microsoft.com/96356a0e-ae0d-4000-9223-a578cbdeaa8b">GetExtendedTcpTable</a>.


## -remarks



This table is specifically returned by a call to <a href="https://msdn.microsoft.com/96356a0e-ae0d-4000-9223-a578cbdeaa8b">GetExtendedTcpTable</a> with the <i>TableClass</i> parameter set to a <b>TCP_TABLE_OWNER_PID_*</b> value from the <a href="https://msdn.microsoft.com/abfaf7e5-7739-4f23-bfb4-09206111599f">TCP_TABLE_CLASS</a> enumeration and the <i>ulAf</i> parameter set to <b>AF_INET4</b>.

The <b>MIB_TCPTABLE_OWNER_PID</b> structure may contain padding for alignment between the <b>dwNumEntries</b> member and the first <a href="https://msdn.microsoft.com/220b69a4-b372-4eff-8d5a-eca0d39b8af9">MIB_TCPROW_OWNER_PID</a> array entry in the <b>table</b> member. Padding for alignment may also be present between the <b>MIB_TCPROW_OWNER_PID</b> array entries in the <b>table</b> member. Any access to a <b>MIB_TCPROW_OWNER_PID</b> array entry should assume  padding may exist. 



On the Microsoft Windows Software Development Kit (SDK) released for Windows Vistaand later, the organization of header files has changed. This  structure is defined in the <i>Tcpmib.h</i> header file, not in the <i>Iprtrmib.h</i> header file. Note that the <i>Tcpmib.h</i> header file is automatically included in <i>Iprtrmib.h</i>, which is automatically included in the <i>Iphlpapi.h</i> header file. The  <i>Tcpmib.h</i> and <i>Iprtrmib.h</i> header files should never be used directly.




## -see-also




<a href="https://msdn.microsoft.com/4896a9f8-0486-4380-bf49-d1c9ef114acc">IP Helper Start Page</a>



<a href="https://msdn.microsoft.com/566bf187-73d0-4d61-be8e-306dc482a005">MIB Reference</a>



<a href="https://msdn.microsoft.com/811a1e41-efce-4e9c-8329-1c6929e12a8d">MIB Structures</a>
 

 

