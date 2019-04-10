---
UID: NS:cfgmgr32.IO_Des_s
title: IO_DES (cfgmgr32.h)
author: windows-sdk-content
description: The IO_DES structure is used for specifying either a resource list or a resource requirements list that describes I/O port usage for a device instance. For more information about resource lists and resource requirements lists, see Hardware Resources.
old-location: devinst\io_des.htm
tech.root: devinst
ms.assetid: 4b2ae544-0254-4221-80df-e2df4a23d15f
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PIO_DES, IO_DES, IO_DES structure [Device and Driver Installation], PIO_DES, PIO_DES structure pointer [Device and Driver Installation], cfgmgr32/IO_DES, cfgmgr32/PIO_DES, cfgmgrst_027e9190-0074-48e2-89cd-aa86e8a08165.xml, devinst.io_des"
ms.topic: struct
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - cfgmgr32.h
api_name:
 - IO_DES
product: Windows
targetos: Windows
req.typenames: IO_DES, *PIO_DES
req.redist: 
---

# IO_DES structure


## -description


The IO_DES structure is used for specifying either a resource list or a resource requirements list that describes I/O port usage for a device instance. For more information about resource lists and resource requirements lists, see <a href="https://msdn.microsoft.com/c7a6997b-34f9-4dd9-b384-2321a8b5ce54">Hardware Resources</a>.


## -struct-fields




### -field IOD_Count





#### For a resource list:

Zero.



#### For a resource requirements list:

The number of elements in the <a href="https://msdn.microsoft.com/1793684b-b4c4-4467-9ac9-8c6b1eea65e3">IO_RANGE</a> array that is included in the <a href="https://msdn.microsoft.com/d18a1f92-b76c-4240-9a0e-7474c258436c">IO_RESOURCE</a> structure.


### -field IOD_Type

Must be set to the constant value <b>IOType_Range</b>.


### -field IOD_Alloc_Base





#### For a resource list:

The lowest-numbered of a range of contiguous I/O port addresses allocated to the device.



#### For a resource requirements list:

Zero.


### -field IOD_Alloc_End





#### For a resource list:

The highest-numbered of a range of contiguous I/O port addresses allocated to the device.



#### For a resource requirements list:

Zero.


### -field IOD_DesFlags

One bit flag from <i>each</i> of the flag sets described in the following table.

<table>
<tr>
<th></th>
<th>Flag</th>
<th>Definition</th>
</tr>
<tr>
<td colspan="2">
<i>Port Type Flags</i>

</td>
<td></td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_IO</b>

</td>
<td>
The device is accessed in I/O address space.

</td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_Memory</b>

</td>
<td>
The device is accessed in memory address space.

</td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_PortType</b>

</td>
<td>
Bitmask for the bits within <b>IOD_DesFlags</b> that specify the port type value.

</td>
</tr>
<tr>
<td colspan="2">
<i>Decode Flags</i>

</td>
<td></td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_10_BIT_DECODE</b>

</td>
<td>
The device decodes 10 bits of the port address.

</td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_12_BIT_DECODE</b>

</td>
<td>
The device decodes 12 bits of the port address.

</td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_16_BIT_DECODE</b>

</td>
<td>
The device decodes 16 bits of the port address.

</td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_POSITIVE_DECODE</b>

</td>
<td>
The device uses "positive decode" instead of "subtractive decode."

</td>
</tr>
<tr>
<td></td>
<td>
<b>fIOD_DECODE</b>

</td>
<td>
Bitmask for the bits within <b>IOD_DesFlags</b> that specify the decode value.

</td>
</tr>
</table>
 


## -see-also




<a href="https://msdn.microsoft.com/1793684b-b4c4-4467-9ac9-8c6b1eea65e3">IO_RANGE</a>



<a href="https://msdn.microsoft.com/d18a1f92-b76c-4240-9a0e-7474c258436c">IO_RESOURCE</a>
 

 

