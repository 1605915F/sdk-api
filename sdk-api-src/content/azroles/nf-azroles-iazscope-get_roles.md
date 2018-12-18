---
UID: NF:azroles.IAzScope.get_Roles
title: IAzScope::get_Roles
author: windows-sdk-content
description: Retrieves an IAzRoles object that is used to enumerate IAzRole objects from the policy data.
old-location: security\iazscope_roles.htm
tech.root: secauthz
ms.assetid: 4dcf0e1b-d824-4675-b2d1-f59a58adb00a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzScope object [Security],Roles property, IAzScope interface [Security],Roles property, IAzScope.Roles, IAzScope.get_Roles, IAzScope::Roles, IAzScope::get_Roles, Roles property [Security], Roles property [Security],AzScope object, Roles property [Security],IAzScope interface, azroles/IAzScope::Roles, azroles/IAzScope::get_Roles, get_Roles, security.iazscope_roles
ms.topic: method
req.header: azroles.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.lib: Azroles.lib
req.dll: Azroles.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Azroles.dll
api_name:
 - IAzScope.Roles
 - IAzScope.get_Roles
 - AzScope.Roles
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzScope::get_Roles


## -description


The <b>Roles</b> property retrieves an <a href="https://msdn.microsoft.com/bc69ec52-ea73-4a0c-a9a2-913a6725489e">IAzRoles</a> object that is used to enumerate <a href="https://msdn.microsoft.com/2934d783-b379-486c-80e7-e7650b89dc1a">IAzRole</a> objects from the policy data.

This property is read-only.


## -parameters


## -remarks



This property can be used only to enumerate <a href="https://msdn.microsoft.com/2934d783-b379-486c-80e7-e7650b89dc1a">IAzRole</a> objects that are direct child objects of the <a href="https://msdn.microsoft.com/f7abe7cb-8827-46f6-85fe-99282582a3d4">IAzScope</a> object.



