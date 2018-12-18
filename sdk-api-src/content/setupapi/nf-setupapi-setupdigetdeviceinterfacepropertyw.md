---
UID: NF:setupapi.SetupDiGetDeviceInterfacePropertyW
title: SetupDiGetDeviceInterfacePropertyW function
author: windows-sdk-content
description: The SetupDiGetDeviceInterfaceProperty function retrieves a device property that is set for a device interface.
old-location: devinst\setupdigetdeviceinterfaceproperty.htm
tech.root: devinst
ms.assetid: 72a44060-cebc-4690-8776-68db76810732
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetupDiGetDeviceInterfaceProperty, SetupDiGetDeviceInterfaceProperty function [Device and Driver Installation], SetupDiGetDeviceInterfacePropertyW, devinst.setupdigetdeviceinterfaceproperty, di-rtns_7a7e0730-650f-4deb-a724-8f90385c762a.xml, setupapi/SetupDiGetDeviceInterfaceProperty
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: DesktopFor universal, call CM_Get_Device_Interface_Property
req.target-min-winverclnt: Available in Windows Vista and later versions of Windows.
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
req.lib: Setupapi.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Setupapi.lib
 - Setupapi.dll
api_name:
 - SetupDiGetDeviceInterfaceProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetupDiGetDeviceInterfacePropertyW function


## -description


The <b>SetupDiGetDeviceInterfaceProperty</b> function retrieves a device property that is set for a device interface.


## -parameters




### -param DeviceInfoSet [in]

A handle to a <a href="https://msdn.microsoft.com/library/Ff541247(v=VS.85).aspx">device information set</a> that contains a device interface for which to retrieve a device interface property.


### -param DeviceInterfaceData [in]

A pointer to an <a href="https://msdn.microsoft.com/df142e95-aa1c-4d3e-90c6-bac86effbd5d">SP_DEVICE_INTERFACE_DATA</a> structure that represents the device interface for which to retrieve a device interface property. 


### -param PropertyKey [in]

A pointer to a <a href="https://msdn.microsoft.com/98986d43-84c0-44e6-83f9-08e872ea5e6d">DEVPROPKEY</a> structure that represents the device interface property key of the device interface property to retrieve. 


### -param PropertyType [out]

A pointer to a <a href="https://msdn.microsoft.com/e0fdcc28-be70-4ae1-bd6d-89e2177eae62">DEVPROPTYPE</a>-typed variable that receives the property-data-type identifier of the requested device interface property. The property-data-type identifier is a bitwise OR between a base-data-type identifier and, if the base-data type is modified, a property-data-type modifier.


### -param PropertyBuffer [out]

A pointer to a buffer that receives the requested device interface property. <b>SetupDiGetDeviceInterfaceProperty</b> retrieves the requested property only if the buffer is large enough to hold all the property value data. The pointer can be <b>NULL</b>. If the pointer is set to <b>NULL</b> and <i>RequiredSize</i> is supplied, <b>SetupDiGetDeviceInterfaceProperty</b> returns the size of the property, in bytes, in *<i>RequiredSize</i>.


### -param PropertyBufferSize [in]

The size, in bytes, of the <i>PropertyBuffer</i> buffer. If <i>PropertyBuffer</i> is set to <b>NULL</b>, <i>PropertyBufferSize</i> must be set to zero.


### -param RequiredSize [out, optional]

A pointer to a DWORD-typed variable that receives the size, in bytes, of either the device interface property if the property is retrieved or the required buffer size, if the buffer is not large enough. This pointer can be set to <b>NULL</b>.


### -param Flags [in]

This parameter must be set to zero.


## -returns



<b>SetupDiGetDeviceInterfaceProperty</b> returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b>, and the logged error can be retrieved by calling <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.

The following table includes some of the more common error codes that this function might log. Other error codes can be set by the device installer functions that are called by this API.


<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_FLAGS</b></dt>
</dl>
</td>
<td width="60%">
The value of<i> Flags</i> is not zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_HANDLE</b></dt>
</dl>
</td>
<td width="60%">
The device information set that is specified by <i>DevInfoSet</i> is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
A supplied parameter is not valid. One possibility is that the device interface that is specified by <i>DeviceInterfaceData</i> is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_REG_PROPERTY</b></dt>
</dl>
</td>
<td width="60%">
The property key that is supplied by <i>PropertyKey</i> is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_DATA</b></dt>
</dl>
</td>
<td width="60%">
An unspecified internal data value was not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_USER_BUFFER</b></dt>
</dl>
</td>
<td width="60%">
A user buffer is not valid. One possibility is that <i>PropertyBuffer</i> is <b>NULL</b>, and <i>PropertyBufferSize</i> is not zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NO_SUCH_DEVICE_INTERFACE</b></dt>
</dl>
</td>
<td width="60%">
The device interface that is specified by <i>DeviceInterfaceData</i> does not exist.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INSUFFICIENT_BUFFER</b></dt>
</dl>
</td>
<td width="60%">
The <i>PropertyBuffer</i> buffer is not large enough to hold the property value, or an internal data buffer that was passed to a system call was too small.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
There was not enough system memory available to complete the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The requested device property does not exist.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The caller does not have Administrator privileges. 

</td>
</tr>
</table>
 




## -remarks



<b>SetupDiGetDeviceInterfaceProperty</b> is part of the <a href="https://msdn.microsoft.com/library/Ff553515(v=VS.85).aspx">unified device property model</a>. 

SetupAPI supports only a Unicode version of <b>SetupDiGetDeviceInterfaceProperty</b>. 

A caller of <b>SetupDiGetDeviceInterfaceProperty</b> must be a member of the Administrators group to set a device interface property. 

To obtain the device property keys that represent the device properties that are set for a device interface, call <a href="https://msdn.microsoft.com/46eedc41-17ee-4306-ad34-22bfd98cb96b">SetupDiGetDeviceInterfacePropertyKeys</a>.

To set a device interface property, call <a href="https://msdn.microsoft.com/5c8da8a3-1c53-42c1-8adc-46743b63f731">SetupDiSetDeviceInterfaceProperty</a>.




## -see-also




<a href="https://msdn.microsoft.com/46eedc41-17ee-4306-ad34-22bfd98cb96b">SetupDiGetDeviceInterfacePropertyKeys</a>



<a href="https://msdn.microsoft.com/5c8da8a3-1c53-42c1-8adc-46743b63f731">SetupDiSetDeviceInterfaceProperty</a>
 

 

