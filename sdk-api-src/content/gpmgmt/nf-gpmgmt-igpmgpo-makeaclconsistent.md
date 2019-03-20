---
UID: NF:gpmgmt.IGPMGPO.MakeACLConsistent
title: IGPMGPO::MakeACLConsistent (gpmgmt.h)
author: windows-sdk-content
description: Makes ACLs consistent on the Directory Service and the system volume folder (SysVol) of the GPO. IsACLConsistent can be used to check for consistency of ACLs between the Directory Service and system volume folder (SysVol).
old-location: gpmc\igpmgpo_makeaclconsistent.htm
tech.root: gpmc
ms.assetid: 936e7795-e5ab-4014-86df-6b74ab122b11
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GPMGPO class [GPMC],MakeACLConsistent method, IGPMGPO interface [GPMC],MakeACLConsistent method, IGPMGPO.MakeACLConsistent, IGPMGPO::MakeACLConsistent, MakeACLConsistent, MakeACLConsistent method [GPMC], MakeACLConsistent method [GPMC],GPMGPO class, MakeACLConsistent method [GPMC],IGPMGPO interface, gpmc.igpmgpo_makeaclconsistent, gpmgmt/IGPMGPO::MakeACLConsistent
ms.topic: method
req.header: gpmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Gpmgmt.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Gpmgmt.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gpmgmt.dll
api_name:
 - IGPMGPO.MakeACLConsistent
 - GPMGPO.MakeACLConsistent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IGPMGPO::MakeACLConsistent


## -description


Makes <a href="https://msdn.microsoft.com/library/Aa374872(v=VS.85).aspx">ACLs</a> consistent on the Directory Service and the system  volume folder (SysVol) of the GPO. <a href="https://msdn.microsoft.com/4a4f2d87-bfaa-453a-9dbe-de19ba1d1953">IsACLConsistent</a> can be used to check for consistency of ACLs between the Directory Service and system volume folder (SysVol).


## -parameters






## -returns



<h3>JScript</h3>
Returns <b>S_OK</b> if successful. Returns a failure code if an error occurs.

<h3>VB</h3>
Returns <b>S_OK</b> if successful. Returns a failure code if an error occurs.




## -remarks



For more information about ACLs and the security model for controlling access to Windows objects, see <a href="https://msdn.microsoft.com/d9ce4ec5-5c09-4b33-93a1-39638a925986">Access Control</a>.




## -see-also




<a href="https://msdn.microsoft.com/2857c8b7-019d-4ec2-9a00-574fc8541cae">IGPMGPO</a>



<a href="https://msdn.microsoft.com/4a4f2d87-bfaa-453a-9dbe-de19ba1d1953">IGPMGPO::IsACLConsistent</a>
 

 

