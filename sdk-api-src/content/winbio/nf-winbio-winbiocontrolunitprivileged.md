---
UID: NF:winbio.WinBioControlUnitPrivileged
title: WinBioControlUnitPrivileged function
author: windows-sdk-content
description: Allows the caller to perform privileged vendor-defined control operations on a biometric unit. Starting with Windows 10, build 1607, this function is available to use with a mobile image.
old-location: secbiomet\winbiocontrolunitprivileged.htm
tech.root: SecBioMet
ms.assetid: 102299e9-3276-4802-bd65-c3dd593f07b8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WINBIO_COMPONENT_ENGINE, WINBIO_COMPONENT_SENSOR, WINBIO_COMPONENT_STORAGE, WinBioControlUnitPrivileged, WinBioControlUnitPrivileged function [Windows Biometric Framework API], secbiomet.winbiocontrolunitprivileged, winbio/WinBioControlUnitPrivileged
ms.topic: function
req.header: winbio.h
req.include-header: Winbio.h
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
req.lib: Winbio.lib
req.dll: Winbio.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Winbio.dll
 - Ext-MS-Win-BioMetrics-WinBio-l1-2-0.dll
 - winbioext.dll
 - Ext-MS-Win-BioMetrics-WinBio-Core-L1-1-0.dll
 - Ext-MS-Win-BioMetrics-WinBio-Core-L1-1-1.dll
api_name:
 - WinBioControlUnitPrivileged
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WinBioControlUnitPrivileged function


## -description


Allows the caller to perform privileged vendor-defined control operations on a biometric unit. Starting with Windows 10, build 1607, this  function is available to use with a mobile image. The client must call this function to perform extended vendor operations that require elevated access rights. If no privileges are required, the client can call the <a href="https://msdn.microsoft.com/5d11f72a-3392-4089-a563-1771f8c2c8f7">WinBioControlUnit</a> function.


## -parameters




### -param SessionHandle [in]

A <b>WINBIO_SESSION_HANDLE</b> value that identifies an open biometric session. Open a synchronous session handle by calling <a href="https://msdn.microsoft.com/e9a0bb5f-4bbd-4dc4-9cd8-c26f5e4f74cf">WinBioOpenSession</a>. Open an asynchronous session handle by calling <a href="https://msdn.microsoft.com/711EDE14-A2EE-415D-8FB6-562D71D68146">WinBioAsyncOpenSession</a>.


### -param UnitId [in]

A <b>WINBIO_UNIT_ID</b> value that identifies the biometric unit. This value must correspond to the unit ID used previously in  the <a href="https://msdn.microsoft.com/421520eb-ae67-4ead-8202-ffa468a20bdd">WinBioLockUnit</a> function.


### -param Component [in]

A <b>WINBIO_COMPONENT</b> value that specifies the component within the biometric unit that should perform the operation. This can be one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="WINBIO_COMPONENT_SENSOR"></a><a id="winbio_component_sensor"></a><dl>
<dt><b>WINBIO_COMPONENT_SENSOR</b></dt>
</dl>
</td>
<td width="60%">
Send the command to the sensor adapter.

</td>
</tr>
<tr>
<td width="40%"><a id="WINBIO_COMPONENT_ENGINE"></a><a id="winbio_component_engine"></a><dl>
<dt><b>WINBIO_COMPONENT_ENGINE</b></dt>
</dl>
</td>
<td width="60%">
Send the command to the engine adapter.

</td>
</tr>
<tr>
<td width="40%"><a id="WINBIO_COMPONENT_STORAGE"></a><a id="winbio_component_storage"></a><dl>
<dt><b>WINBIO_COMPONENT_STORAGE</b></dt>
</dl>
</td>
<td width="60%">
Send the command to the storage adapter.

</td>
</tr>
</table>
 


### -param ControlCode [in]

A vendor-defined code recognized by the biometric unit specified by the <i>UnitId</i> parameter and the adapter specified by the <i>Component</i> parameter.


### -param SendBuffer

Address of the buffer that contains the control information to be sent to the adapter specified by the <i>Component</i> parameter. The format and content of the buffer is vendor-defined.


### -param SendBufferSize [in]

Size, in bytes, of the buffer specified by the <i>SendBuffer</i> parameter.


### -param ReceiveBuffer

Address of the buffer that receives information sent by the adapter specified by the <i>Component</i> parameter. The format and content of the buffer is vendor-defined.


### -param ReceiveBufferSize [in]

Size, in bytes, of the buffer specified by the <i>ReceiveBuffer</i> parameter.


### -param ReceiveDataSize

Pointer to a <b>SIZE_T</b> value that contains the size, in bytes, of the data written to the buffer specified by the <i>ReceiveBuffer</i> parameter.


### -param OperationStatus [out, optional]

Pointer to an integer that contains a vendor-defined status code that specifies the outcome of the control operation.


## -returns



If the function succeeds, it returns S_OK. If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following table.  For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>E_HANDLE</b></b></dt>
</dl>
</td>
<td width="60%">
The session handle is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>E_INVALIDARG</b></b></dt>
</dl>
</td>
<td width="60%">
The value specified in the <i>ControlCode</i> parameter is not recognized.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>E_POINTER</b></b></dt>
</dl>
</td>
<td width="60%">
The <i>SendBuffer</i>, <i>ReceiveBuffer</i>, <i>ReceiveDataSize</i>, <i>OperationStatus</i> parameters cannot be <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>E_ACCESSDENIED</b></b></dt>
</dl>
</td>
<td width="60%">
The caller does not have permission to perform the operation, or the session was not opened by using <b>WINBIO_FLAG_MAINTENANCE</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>E_INVALIDARG</b></b></dt>
</dl>
</td>
<td width="60%">
The value specified in the <i>ControlCode</i> parameter is not recognized.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>WINBIO_E_LOCK_VIOLATION</b></b></dt>
</dl>
</td>
<td width="60%">
The biometric unit specified by the <i>UnitId</i> parameter must be locked before any control operations can be performed.

</td>
</tr>
</table>
 




## -remarks



Vendors who create plug-ins must decide which extended operations are privileged and which are available to all clients. To perform a privileged operation, the client application must call the <b>WinBioControlUnitPrivileged</b> function. The Windows Biometric Framework allows only clients that have the appropriate access rights to call this function. To perform an operation that does not require privileges, the client should call the <a href="https://msdn.microsoft.com/5d11f72a-3392-4089-a563-1771f8c2c8f7">WinBioControlUnit</a> function.

You must call <a href="https://msdn.microsoft.com/421520eb-ae67-4ead-8202-ffa468a20bdd">WinBioLockUnit</a> before calling <b>WinBioControlUnitPrivileged</b>. The <b>WinBioLockUnit</b> function creates a locked region in which vendor-defined operations can be securely performed.

To call this function successfully, the session handle must have been opened by specifying <b>WINBIO_FLAG_MAINTENANCE</b>. Only the Administrators and Local System accounts have the necessary privileges.

To use <b>WinBioControlUnitPrivileged</b> synchronously, call the function with a session handle created by calling <a href="https://msdn.microsoft.com/e9a0bb5f-4bbd-4dc4-9cd8-c26f5e4f74cf">WinBioOpenSession</a>. The function blocks until the operation completes or an error is encountered.

To use <b>WinBioControlUnitPrivileged</b> asynchronously, call the function with a session handle created by calling <a href="https://msdn.microsoft.com/711EDE14-A2EE-415D-8FB6-562D71D68146">WinBioAsyncOpenSession</a>. The framework allocates a <a href="https://msdn.microsoft.com/1C8A4557-3851-4AB2-BB9B-AE199EB9D024">WINBIO_ASYNC_RESULT</a> structure  and uses it to return information about operation success or failure. The <b>WINBIO_ASYNC_RESULT</b> structure is returned to the application callback or to the application message queue, depending on the value you set in the <i>NotificationMethod</i> parameter of the <b>WinBioAsyncOpenSession</b> function.

<ul>
<li>If you choose to receive completion notices by using a callback, you must implement a <a href="https://msdn.microsoft.com/550EA13D-18CE-4B73-9C9B-4D5C46C48A75">PWINBIO_ASYNC_COMPLETION_CALLBACK</a> function and set the  <i>NotificationMethod</i> parameter to <b>WINBIO_ASYNC_NOTIFY_CALLBACK</b>.</li>
<li>If you choose to receive completion notices by using the application message queue, you must set the  <i>NotificationMethod</i> parameter to <b>WINBIO_ASYNC_NOTIFY_MESSAGE</b>. The framework returns a <a href="https://msdn.microsoft.com/1C8A4557-3851-4AB2-BB9B-AE199EB9D024">WINBIO_ASYNC_RESULT</a> pointer to the <b>LPARAM</b> field of the window message.</li>
</ul>
To prevent memory leaks, you must call <a href="https://msdn.microsoft.com/b570fc6c-a08e-4485-a621-20f59bd63d40">WinBioFree</a> to release the <a href="https://msdn.microsoft.com/1C8A4557-3851-4AB2-BB9B-AE199EB9D024">WINBIO_ASYNC_RESULT</a> structure after you have finished using it.




## -see-also




<a href="https://msdn.microsoft.com/5d11f72a-3392-4089-a563-1771f8c2c8f7">WinBioControlUnit</a>



<a href="https://msdn.microsoft.com/421520eb-ae67-4ead-8202-ffa468a20bdd">WinBioLockUnit</a>
 

 

