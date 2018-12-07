---
UID: NF:certenroll.ICryptAttribute.get_ObjectId
title: ICryptAttribute::get_ObjectId
author: windows-sdk-content
description: Retrieves the object identifier (OID) for the attribute.
old-location: security\icryptattribute_objectid_property.htm
tech.root: seccertenroll
ms.assetid: 9ae9a217-1658-42ac-bd28-33abab5d0d70
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICryptAttribute interface [Security],ObjectId property, ICryptAttribute.ObjectId, ICryptAttribute.get_ObjectId, ICryptAttribute::ObjectId, ICryptAttribute::get_ObjectId, ObjectId property [Security], ObjectId property [Security],ICryptAttribute interface, certenroll/ICryptAttribute::ObjectId, certenroll/ICryptAttribute::get_ObjectId, get_ObjectId, security.icryptattribute_objectid_property
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenroll.h
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
req.dll: CertEnroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CertEnroll.dll
api_name:
 - ICryptAttribute.ObjectId
 - ICryptAttribute.get_ObjectId
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICryptAttribute::get_ObjectId


## -description


The <b>ObjectId</b> property retrieves the <a href="https://msdn.microsoft.com/en-us/library/ms721599(v=VS.85).aspx">object identifier</a> (OID) for the attribute.

This property is read-only.


## -parameters


## -remarks



 You can initialize an <a href="https://msdn.microsoft.com/en-us/library/Aa376784(v=VS.85).aspx">IObjectId</a> object by calling <a href="https://msdn.microsoft.com/en-us/library/Aa376797(v=VS.85).aspx">InitializeFromName</a>. This method initializes the object by using a value from the <a href="https://msdn.microsoft.com/en-us/library/Aa374855(v=VS.85).aspx">CERTENROLL_OBJECTID</a> enumeration. The enumeration value is associated with an ASN.1 object identifier. For example, the value <b>XCN_OID_COUNTRY_NAME</b> is associated with a string containing 2.5.4.6. This is the dotted decimal representation of the joint-iso-itu-t(2)ds(5)attributeType(4)countryName(6) object identifier.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa375929(v=VS.85).aspx">ICryptAttribute</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa375930(v=VS.85).aspx">ICryptAttributes</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa377058(v=VS.85).aspx">IX509Attribute</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa377108(v=VS.85).aspx">IX509Attributes</a>
 

 

