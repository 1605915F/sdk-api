---
UID: NF:powerbase.CallNtPowerInformation
title: CallNtPowerInformation function
author: windows-sdk-content
description: Sets or retrieves power information.
old-location: base\callntpowerinformation.htm
tech.root: power
ms.assetid: adc0052d-e2dd-4c55-996c-6af8f5987d79
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AdministratorPowerPolicy, CallNtPowerInformation, CallNtPowerInformation function, LastSleepTime, LastWakeTime, ProcessorInformation, ProcessorPowerPolicyAc, ProcessorPowerPolicyCurrent, ProcessorPowerPolicyDc, SystemBatteryState, SystemExecutionState, SystemPowerCapabilities, SystemPowerInformation, SystemPowerPolicyAc, SystemPowerPolicyCurrent, SystemPowerPolicyDc, SystemReserveHiberFile, VerifyProcessorPowerPolicyAc, VerifyProcessorPowerPolicyDc, VerifySystemPolicyAc, VerifySystemPolicyDc, _win32_callntpowerinformation, base.callntpowerinformation, powerbase/CallNtPowerInformation, powrprof/CallNtPowerInformation
ms.topic: function
req.header: powerbase.h
req.include-header: 
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
req.lib: PowrProf.lib
req.dll: PowrProf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - PowrProf.dll
 - API-MS-Win-power-base-l1-1-0.dll
api_name:
 - CallNtPowerInformation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CallNtPowerInformation function


## -description


Sets or retrieves power information.


## -parameters




### -param InformationLevel [in]

The information level requested. This value indicates the specific power information to be set or 
      retrieved. This parameter must be one of the following 
      <b>POWER_INFORMATION_LEVEL</b> enumeration type values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="AdministratorPowerPolicy"></a><a id="administratorpowerpolicy"></a><a id="ADMINISTRATORPOWERPOLICY"></a><dl>
<dt><b>AdministratorPowerPolicy</b></dt>
<dt>9</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
        
       

</td>
</tr>
<tr>
<td width="40%"><a id="LastSleepTime"></a><a id="lastsleeptime"></a><a id="LASTSLEEPTIME"></a><dl>
<dt><b>LastSleepTime</b></dt>
<dt>15</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>; otherwise, the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives a <b>ULONGLONG</b> that 
         specifies the interrupt-time count, in 100-nanosecond units, at the last system sleep time.

</td>
</tr>
<tr>
<td width="40%"><a id="LastWakeTime"></a><a id="lastwaketime"></a><a id="LASTWAKETIME"></a><dl>
<dt><b>LastWakeTime</b></dt>
<dt>14</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>; otherwise, the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives a <b>ULONGLONG</b> that 
         specifies the interrupt-time count, in 100-nanosecond units, at the last system wake time.

</td>
</tr>
<tr>
<td width="40%"><a id="ProcessorInformation"></a><a id="processorinformation"></a><a id="PROCESSORINFORMATION"></a><dl>
<dt><b>ProcessorInformation</b></dt>
<dt>11</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>; otherwise the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives one 
         <a href="https://msdn.microsoft.com/fa8c533c-3a54-4eb5-893f-649dfd8b4609">PROCESSOR_POWER_INFORMATION</a> 
         structure for each processor that is installed on the system. Use the <a href="https://msdn.microsoft.com/f6d745af-729a-494e-90b4-19fe7d97c7af">GetSystemInfo</a> function to retrieve the number of processors.

</td>
</tr>
<tr>
<td width="40%"><a id="ProcessorPowerPolicyAc"></a><a id="processorpowerpolicyac"></a><a id="PROCESSORPOWERPOLICYAC"></a><dl>
<dt><b>ProcessorPowerPolicyAc</b></dt>
<dt>18</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
        
       

</td>
</tr>
<tr>
<td width="40%"><a id="ProcessorPowerPolicyCurrent"></a><a id="processorpowerpolicycurrent"></a><a id="PROCESSORPOWERPOLICYCURRENT"></a><dl>
<dt><b>ProcessorPowerPolicyCurrent</b></dt>
<dt>22</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
        
       

</td>
</tr>
<tr>
<td width="40%"><a id="ProcessorPowerPolicyDc"></a><a id="processorpowerpolicydc"></a><a id="PROCESSORPOWERPOLICYDC"></a><dl>
<dt><b>ProcessorPowerPolicyDc</b></dt>
<dt>19</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
        
       

</td>
</tr>
<tr>
<td width="40%"><a id="SystemBatteryState"></a><a id="systembatterystate"></a><a id="SYSTEMBATTERYSTATE"></a><dl>
<dt><b>SystemBatteryState</b></dt>
<dt>5</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>; otherwise, the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives a 
         <a href="https://msdn.microsoft.com/en-us/library/Aa373212(v=VS.85).aspx">SYSTEM_BATTERY_STATE</a> structure containing 
         information about the current system battery.

</td>
</tr>
<tr>
<td width="40%"><a id="SystemExecutionState"></a><a id="systemexecutionstate"></a><a id="SYSTEMEXECUTIONSTATE"></a><dl>
<dt><b>SystemExecutionState</b></dt>
<dt>16</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>; otherwise the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives a <b>ULONG</b> value 
         containing the system execution state buffer. This value may contain any combination of the following values: 
         <b>ES_SYSTEM_REQUIRED</b>, <b>ES_DISPLAY_REQUIRED</b>, or 
         <b>ES_USER_PRESENT</b>. For more information, see the 
         <a href="https://msdn.microsoft.com/9214ea84-7636-4a78-91fd-a5a5da8199a1">SetThreadExecutionState</a> function.

</td>
</tr>
<tr>
<td width="40%"><a id="SystemPowerCapabilities"></a><a id="systempowercapabilities"></a><a id="SYSTEMPOWERCAPABILITIES"></a><dl>
<dt><b>SystemPowerCapabilities</b></dt>
<dt>4</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>, otherwise, the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives a 
         <a href="https://msdn.microsoft.com/en-us/library/Aa373215(v=VS.85).aspx">SYSTEM_POWER_CAPABILITIES</a> structure 
         containing the current system power capabilities.

This information represents the currently supported power capabilities. It may change as drivers are 
         installed in the system. For example, installation of legacy device drivers that do not support power 
         management disables all system sleep states.

</td>
</tr>
<tr>
<td width="40%"><a id="SystemPowerInformation"></a><a id="systempowerinformation"></a><a id="SYSTEMPOWERINFORMATION"></a><dl>
<dt><b>SystemPowerInformation</b></dt>
<dt>12</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>; otherwise, the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives a 
         <a href="https://msdn.microsoft.com/f6349b7c-1835-4492-95e3-9ce142628804">SYSTEM_POWER_INFORMATION</a> structure.

Applications can use this level to retrieve information about the idleness of the system.

</td>
</tr>
<tr>
<td width="40%"><a id="SystemPowerPolicyAc"></a><a id="systempowerpolicyac"></a><a id="SYSTEMPOWERPOLICYAC"></a><dl>
<dt><b>SystemPowerPolicyAc</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
If <i>lpInBuffer</i> is not <b>NULL</b>, the function applies the 
        <a href="https://msdn.microsoft.com/0e73e94d-e529-46fb-b3e5-a79ba2c05713">SYSTEM_POWER_POLICY</a> values passed in 
        <i>lpInBuffer</i> to the current system power policy used while the system is running on AC 
        (utility) power.
        

The <i>lpOutputBuffer</i> buffer receives a 
         <a href="https://msdn.microsoft.com/0e73e94d-e529-46fb-b3e5-a79ba2c05713">SYSTEM_POWER_POLICY</a> structure containing 
         the current system power policy used while the system is running on AC (utility) power.

</td>
</tr>
<tr>
<td width="40%"><a id="SystemPowerPolicyCurrent"></a><a id="systempowerpolicycurrent"></a><a id="SYSTEMPOWERPOLICYCURRENT"></a><dl>
<dt><b>SystemPowerPolicyCurrent</b></dt>
<dt>8</dt>
</dl>
</td>
<td width="60%">
The <i>lpInBuffer</i> parameter must be <b>NULL</b>; otherwise, the 
        function returns <b>ERROR_INVALID_PARAMETER</b>.
        

The <i>lpOutputBuffer</i> buffer receives a 
         <a href="https://msdn.microsoft.com/0e73e94d-e529-46fb-b3e5-a79ba2c05713">SYSTEM_POWER_POLICY</a> structure 
         containing the current system power policy used while the system is running on AC (utility) power.

</td>
</tr>
<tr>
<td width="40%"><a id="SystemPowerPolicyDc"></a><a id="systempowerpolicydc"></a><a id="SYSTEMPOWERPOLICYDC"></a><dl>
<dt><b>SystemPowerPolicyDc</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
If <i>lpInBuffer</i> is not <b>NULL</b>, the function applies the 
        <a href="https://msdn.microsoft.com/0e73e94d-e529-46fb-b3e5-a79ba2c05713">SYSTEM_POWER_POLICY</a> values 
        passed in <i>lpInBuffer</i> to the current system power policy used while the system is 
        running on battery power.
        

The <i>lpOutputBuffer</i> buffer receives a 
         <a href="https://msdn.microsoft.com/0e73e94d-e529-46fb-b3e5-a79ba2c05713">SYSTEM_POWER_POLICY</a> structure containing 
         the current system power policy used while the system is running on battery power.

</td>
</tr>
<tr>
<td width="40%"><a id="SystemReserveHiberFile"></a><a id="systemreservehiberfile"></a><a id="SYSTEMRESERVEHIBERFILE"></a><dl>
<dt><b>SystemReserveHiberFile</b></dt>
<dt>10</dt>
</dl>
</td>
<td width="60%">
If <i>lpInBuffer</i> is not <b>NULL</b> and the current user has 
        sufficient privileges, the function commits or decommits the storage required to hold the hibernation image on 
        the boot volume.
        

The <i>lpInBuffer</i> parameter must point to a <b>BOOLEAN</b> 
         value indicating the desired request. If the value is <b>TRUE</b>, the hibernation file is 
         reserved; if the value is <b>FALSE</b>, the hibernation file is removed.

</td>
</tr>
<tr>
<td width="40%"><a id="VerifyProcessorPowerPolicyAc"></a><a id="verifyprocessorpowerpolicyac"></a><a id="VERIFYPROCESSORPOWERPOLICYAC"></a><dl>
<dt><b>VerifyProcessorPowerPolicyAc</b></dt>
<dt>20</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
         
       

</td>
</tr>
<tr>
<td width="40%"><a id="VerifyProcessorPowerPolicyDc"></a><a id="verifyprocessorpowerpolicydc"></a><a id="VERIFYPROCESSORPOWERPOLICYDC"></a><dl>
<dt><b>VerifyProcessorPowerPolicyDc</b></dt>
<dt>21</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
        
       

</td>
</tr>
<tr>
<td width="40%"><a id="VerifySystemPolicyAc"></a><a id="verifysystempolicyac"></a><a id="VERIFYSYSTEMPOLICYAC"></a><dl>
<dt><b>VerifySystemPolicyAc</b></dt>
<dt>2</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
        
							

</td>
</tr>
<tr>
<td width="40%"><a id="VerifySystemPolicyDc"></a><a id="verifysystempolicydc"></a><a id="VERIFYSYSTEMPOLICYDC"></a><dl>
<dt><b>VerifySystemPolicyDc</b></dt>
<dt>3</dt>
</dl>
</td>
<td width="60%">
This information level is not supported.
        
							

</td>
</tr>
</table>
 


### -param InputBuffer [in]

A pointer to an optional input buffer. The data type of this buffer depends on the information level 
      requested in the <i>InformationLevel</i> parameter.


### -param InputBufferLength [in]

The size of the input buffer, in bytes.


### -param OutputBuffer [out]

A pointer to an optional output buffer. The data type of this buffer depends on the information level 
      requested in the <i>InformationLevel</i> parameter. If the buffer is too small to contain the 
      information, the function returns STATUS_BUFFER_TOO_SMALL.


### -param OutputBufferLength [in]

The size of the output buffer, in bytes. Depending on the information level requested, this may be a 
      variably sized buffer.


## -returns



If the function succeeds, the return value is <b>STATUS_SUCCESS</b>.

If the function fails, the return value can be one the following status codes.

<table>
<tr>
<th>Status</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_BUFFER_TOO_SMALL</b></dt>
</dl>
</td>
<td width="60%">
The output buffer is of insufficient size to contain the data to be returned.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The caller had insufficient access rights to perform the requested action.

</td>
</tr>
</table>
 




## -remarks



Changes made to the current system power policy using 
    <b>CallNtPowerInformation</b> are immediate, but they 
    are not persistent; that is, the changes are not stored as part of a power scheme. Any changes to system power 
    policy made with <b>CallNtPowerInformation</b> may be 
    overwritten by changes to a policy scheme made by the user in the Power Options control panel program, or by 
    subsequent calls to <a href="https://msdn.microsoft.com/b9233601-6848-41c4-bb58-27decad60ba5">WritePwrScheme</a>, 
    <a href="https://msdn.microsoft.com/f449ff0d-5c22-4c6d-8c88-dc18258a8c6d">SetActivePwrScheme</a>, or other power scheme 
    functions.

For more information on using PowrProf.h, see <a href="https://msdn.microsoft.com/36052517-a85c-4512-8772-8aec31551c77">Power 
    Schemes</a>.




## -see-also




<a href="https://msdn.microsoft.com/abd2e2c5-1056-4985-ae07-a40d53bb17b1">ADMINISTRATOR_POWER_POLICY</a>



<a href="https://msdn.microsoft.com/fa8c533c-3a54-4eb5-893f-649dfd8b4609">PROCESSOR_POWER_INFORMATION</a>



<a href="https://msdn.microsoft.com/ea1eae62-26b4-4f5d-a9ca-0a7bb463b90a">PROCESSOR_POWER_POLICY</a>



<a href="https://msdn.microsoft.com/eae96a9e-ced2-4e13-b250-33c5acbbae48">Power Management Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa373212(v=VS.85).aspx">SYSTEM_BATTERY_STATE</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa373215(v=VS.85).aspx">SYSTEM_POWER_CAPABILITIES</a>



<a href="https://msdn.microsoft.com/f6349b7c-1835-4492-95e3-9ce142628804">SYSTEM_POWER_INFORMATION</a>



<a href="https://msdn.microsoft.com/0e73e94d-e529-46fb-b3e5-a79ba2c05713">SYSTEM_POWER_POLICY</a>
 

 

