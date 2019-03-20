---
UID: NS:evntcons._EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID
title: EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID (evntcons.h)
author: windows-sdk-content
description: Defines the parent event of this event.
old-location: etw\event_extended_item_related_activityid.htm
tech.root: ETW
ms.assetid: cabc11ca-e65e-4ffd-9832-7fb4f77417e4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PEVENT_EXTENDED_ITEM_RELATED_ACTIVITYID, EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID, EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID structure [ETW], PEVENT_EXTENDED_ITEM_RELATED_ACTIVITYID, PEVENT_EXTENDED_ITEM_RELATED_ACTIVITYID structure pointer [ETW], base.event_extended_item_related_activityid, etw.event_extended_item_related_activityid, evntcons/EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID, evntcons/PEVENT_EXTENDED_ITEM_RELATED_ACTIVITYID"
ms.topic: struct
req.header: evntcons.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - Evntcons.h
api_name:
 - EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID
product: Windows
targetos: Windows
req.typenames: EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID, *PEVENT_EXTENDED_ITEM_RELATED_ACTIVITYID
req.redist: 
---

# EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID structure


## -description


The <b>EVENT_EXTENDED_ITEM_RELATED_ACTIVITYID</b> structure defines the parent event of this event.


## -struct-fields




### -field RelatedActivityId

A GUID that uniquely identifies the parent activity to which this activity is related. The identifier is specified in the <i>RelatedActivityId</i> parameter passed to the <a href="https://msdn.microsoft.com/798cf3ba-e1cc-4eaf-a1d2-2313a64aab1a">EventWriteTransfer</a> function.


## -see-also




<a href="https://msdn.microsoft.com/130dc14b-7488-48ab-a31d-310c0f4ee13f">EVENT_HEADER_EXTENDED_DATA_ITEM</a>



<a href="https://msdn.microsoft.com/798cf3ba-e1cc-4eaf-a1d2-2313a64aab1a">EventWriteTransfer</a>
 

 

