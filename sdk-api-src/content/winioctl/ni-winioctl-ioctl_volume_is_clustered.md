---
UID: NI:winioctl.IOCTL_VOLUME_IS_CLUSTERED
title: IOCTL_VOLUME_IS_CLUSTERED (winioctl.h)
author: windows-sdk-content
description: Determines whether the specified volume is clustered.
old-location: fs\ioctl_volume_is_clustered.htm
tech.root: FileIO
ms.assetid: 3722b08c-237d-4551-b75e-1d28fe8e94c3
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IOCTL_VOLUME_IS_CLUSTERED, IOCTL_VOLUME_IS_CLUSTERED control, IOCTL_VOLUME_IS_CLUSTERED control code [Files], _win32_ioctl_volume_is_clustered, base.ioctl_volume_is_clustered, fs.ioctl_volume_is_clustered, winioctl/IOCTL_VOLUME_IS_CLUSTERED
ms.topic: ioctl
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - WinIoCtl.h
api_name:
 - IOCTL_VOLUME_IS_CLUSTERED
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCTL_VOLUME_IS_CLUSTERED IOCTL


## -description


Determines whether the specified volume is clustered.

To perform this operation, call the 
<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a> function with the following parameters.

```cpp
BOOL DeviceIoControl(
  (HANDLE) hDevice,            // handle to device
  IOCTL_VOLUME_IS_CLUSTERED,   // dwIoControlCodeNULL,                        // lpInBuffer0,                           // nInBufferSizeNULL,                        // lpOutBuffer0,                           // nOutBufferSize(LPDWORD) lpBytesReturned,   // number of bytes returned
  (LPOVERLAPPED) lpOverlapped  // OVERLAPPED structure
);
```



## -ioctlparameters




### -input-buffer



<text></text>




### -input-buffer-length



<text></text>




### -output-buffer



<text></text>




### -output-buffer-length



<text></text>




### -in-out-buffer



<text></text>




### -inout-buffer-length



<text></text>




### -status-block



Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.

Otherwise, Status to the appropriate error condition as a NTSTATUS code. 

For more information, see [NTSTATUS Values](https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/ntstatus-values).




## -remarks



The 
<b>IOCTL_VOLUME_IS_CLUSTERED</b> control code is valid only if the Cluster service is running.

The <b>ERROR_GEN_FAILURE</b> error indicates that the computer that currently owns the disk on which the volume resides is a server cluster node, but either the disk is a Physical Disk resource currently in an offline state or the disk is not a Physical Disk resource. To determine which of these situations exists, use the following steps:

<ol>
<li>Call the 
<a href="https://msdn.microsoft.com/a7511ac6-04cb-407b-90aa-3382c5160cb6">ClusterEnum</a> function to enumerate all Physical Disk resources in the cluster.</li>
<li>Search each enumerated Physical Disk resource for the volume by calling the 
<a href="https://msdn.microsoft.com/a98ca55a-6535-48cf-a925-5005baa01b94">ClusterResourceControl</a> function with <a href="https://msdn.microsoft.com/e80dfab7-448a-4d68-aae8-c6b42c5dc6f9">CLUSCTL_RESOURCE_STORAGE_GET_DISK_INFO</a>. If you cannot find the volume among the Physical Disk resources in the cluster, the volume does not reside on a Physical Disk resource.</li>
</ol>
The <b>ERROR_INVALID_FUNCTION</b> error indicates that the computer that currently owns the disk on which the volume resides is not a server cluster node or the disk is not a Physical Disk resource. To determine whether a computer is a server cluster node, call the 
<a href="https://msdn.microsoft.com/67534bc8-f19e-4330-850a-788a7f031f5b">GetNodeClusterState</a> function.

In Windows 8 and Windows Server 2012, this code is supported by the following technologies.

<table>
<tr>
<th>Technology</th>
<th>Supported</th>
</tr>
<tr>
<td>
Server Message Block (SMB) 3.0 protocol

</td>
<td>
No

</td>
</tr>
<tr>
<td>
SMB 3.0 Transparent Failover (TFO)

</td>
<td>
No

</td>
</tr>
<tr>
<td>
SMB 3.0 with Scale-out File Shares (SO)

</td>
<td>
No

</td>
</tr>
<tr>
<td>
Cluster Shared Volume File System (CsvFS)

</td>
<td>
Yes

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a>



<a href="https://msdn.microsoft.com/87f39e1c-3ebf-4c6f-a842-699ec3c45e76">Volume
		  Management Control Codes</a>
 

 

