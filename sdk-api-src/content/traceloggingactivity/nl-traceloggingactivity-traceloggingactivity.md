---
UID: NL:traceloggingactivity.TraceLoggingActivity
title: TraceLoggingActivity (traceloggingactivity.h)
author: windows-sdk-content
description: Provides support for logging ETW events during an activity. All events must be manually tagged or nested.
old-location: tracelogging\traceloggingactivity.htm
tech.root: tracelogging
ms.assetid: 75930876-4DF2-4559-BA06-133FC676B1AD
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TraceLoggingActivity, TraceLoggingActivity class, TraceLoggingActivity class,described, tracelogging.traceloggingactivity, traceloggingactivity/TraceLoggingActivity
ms.topic: class
req.header: traceloggingactivity.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2012 R2
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
 - COM
api_location:
 - traceloggingactivity.h
api_name:
 - TraceLoggingActivity
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TraceLoggingActivity class


## -description


Provides support for logging ETW events during an activity. All events must be manually tagged or nested.

<b xmlns:loc="http://microsoft.com/wdcml/l10n">TraceLoggingActivity</b> has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Constructors</a></li>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul><h3><a id="constructors"></a>Constructors</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">TraceLoggingActivity</b> class has these constructors.
<table class="members" id="memberListConstructors">
<tr>
<th align="left" width="37%">Constructor</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn904604(v=VS.85).aspx">TraceLoggingActivity Constructor</a>
</td>
<td align="left" width="63%">
Creates a new <b>TraceLoggingActivity</b> object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn904604(v=VS.85).aspx">TraceLoggingActivity Constructor</a>
</td>
<td align="left" width="63%">
Transfers ownership of an activity from an existing instance to this instance.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn904604(v=VS.85).aspx">TraceLoggingActivity Destructor</a>
</td>
<td align="left" width="63%">
Writes a default stop event if the activity has been started, but has not been stopped.

</td>
</tr>
</table> 
<h3><a id="methods"></a>Methods</h3>The <b>TraceLoggingActivity</b> class has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E9EA0054-DE9B-490A-AD27-BA792B9238EE">TraceLoggingActivity::Id</a>
</td>
<td align="left" width="63%">
Returns a pointer to the activity’s unique identifier (GUID). 

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/C1AC8BBF-E559-4C33-80B2-DDF2F44B37BD">TraceLoggingActivity::IsStarted</a>
</td>
<td align="left" width="63%">
Returns true if the activity has been started.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn975134(v=VS.85).aspx">TraceLoggingActivity::Provider</a>
</td>
<td align="left" width="63%">
Returns the handle to the TraceLogging provider associated with this activity.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn904602(v=VS.85).aspx">TraceLoggingActivity::SetRelatedActivity</a>
</td>
<td align="left" width="63%">
Sets the related activity.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn904603(v=VS.85).aspx">TraceLoggingActivity::SetRelatedActivityId</a>
</td>
<td align="left" width="63%">
Sets the related activity using the unique identifier.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">TraceLoggingActivity</b> class has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/DFD096D7-187D-4DC2-A502-C45362FE2A7A">Keyword constant</a>


</td>
<td align="left" width="63%">
The value of the keyword that will be used in the activity’s start and stop events.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/DBBBE6C8-B952-493F-AE98-89D54536F1E5">Level constant</a>


</td>
<td align="left" width="63%">
Contains the value of the level that will be used in the activity’s start and stop events.

</td>
</tr>
</table> 


## -members

The <b>TraceLoggingActivity</b> class has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E9EA0054-DE9B-490A-AD27-BA792B9238EE">TraceLoggingActivity::Id</a>
</td>
<td align="left" width="63%">
Returns a pointer to the activity’s unique identifier (GUID). 

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/C1AC8BBF-E559-4C33-80B2-DDF2F44B37BD">TraceLoggingActivity::IsStarted</a>
</td>
<td align="left" width="63%">
Returns true if the activity has been started.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn975134(v=VS.85).aspx">TraceLoggingActivity::Provider</a>
</td>
<td align="left" width="63%">
Returns the handle to the TraceLogging provider associated with this activity.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn904602(v=VS.85).aspx">TraceLoggingActivity::SetRelatedActivity</a>
</td>
<td align="left" width="63%">
Sets the related activity.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn904603(v=VS.85).aspx">TraceLoggingActivity::SetRelatedActivityId</a>
</td>
<td align="left" width="63%">
Sets the related activity using the unique identifier.

</td>
</tr>
</table>Returns a pointer to the activity’s unique identifier (GUID). 

Returns true if the activity has been started.

Returns the handle to the TraceLogging provider associated with this activity.

Sets the related activity.

Sets the related activity using the unique identifier.

 

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">TraceLoggingActivity</b> class has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/DFD096D7-187D-4DC2-A502-C45362FE2A7A">Keyword constant</a>


</td>
<td align="left" width="63%">
The value of the keyword that will be used in the activity’s start and stop events.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/DBBBE6C8-B952-493F-AE98-89D54536F1E5">Level constant</a>


</td>
<td align="left" width="63%">
Contains the value of the level that will be used in the activity’s start and stop events.

</td>
</tr>
</table>
<a href="https://msdn.microsoft.com/DFD096D7-187D-4DC2-A502-C45362FE2A7A">Keyword constant</a>


The value of the keyword that will be used in the activity’s start and stop events.


<a href="https://msdn.microsoft.com/DBBBE6C8-B952-493F-AE98-89D54536F1E5">Level constant</a>


Contains the value of the level that will be used in the activity’s start and stop events.

 


## -remarks



In order to use TraceLogging activities, you need to define an instance of either <b>TraceLoggingActivity</b> or <a href="https://msdn.microsoft.com/en-us/library/Dn904612(v=VS.85).aspx">TraceLoggingThreadActivity</a>. After you have created an instance of one of these classes, you manipulate activity logging using <a href="https://msdn.microsoft.com/70382367-E0A0-4E5B-A14F-863BEC0615C5">TraceLoggingFunction</a>, <a href="https://msdn.microsoft.com/E5B9347E-50A7-49BE-BDD5-DCED39371234">TraceLoggingWriteStart</a>, <a href="https://msdn.microsoft.com/638F08E3-5970-40B3-8025-E3D81ECA1D2A">TraceLoggingWriteStop</a>, and <a href="https://msdn.microsoft.com/BBDFC2B1-33C6-4D5F-AA7B-91BB2A757B1E">TraceLoggingWriteTagged</a>. This class automatically creates a unique identifier when it is started and tracing is turned on.
         

You can nest activities manually by providing unique identifiers to the <a href="https://msdn.microsoft.com/E5B9347E-50A7-49BE-BDD5-DCED39371234">TraceLoggingWriteStart</a> and <a href="https://msdn.microsoft.com/638F08E3-5970-40B3-8025-E3D81ECA1D2A">TraceLoggingWriteStop</a> macros.
         




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn904612(v=VS.85).aspx">TraceLoggingThreadActivity Class</a>
 

 

