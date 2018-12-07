---
UID: NF:taskschd.IEmailAction.get_Server
title: IEmailAction::get_Server
author: windows-sdk-content
description: Gets or sets the name of the SMTP server that you use to send email from.
old-location: taskschd\iemailaction_server.htm
tech.root: taskschd
ms.assetid: c781f189-f27b-4f37-af53-144e1ae8cb75
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEmailAction interface [Task Scheduler],Server property, IEmailAction.Server, IEmailAction.get_Server, IEmailAction::Server, IEmailAction::get_Server, IEmailAction::put_Server, Server property [Task Scheduler], Server property [Task Scheduler],IEmailAction interface, get_Server, taskschd.iemailaction_server, taskschd/IEmailAction::Server, taskschd/IEmailAction::get_Server, taskschd/IEmailAction::put_Server
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: taskschd.h
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
req.lib: Taskschd.lib
req.dll: Taskschd.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - taskschd.dll
api_name:
 - IEmailAction.Server
 - IEmailAction.get_Server
 - IEmailAction.put_Server
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEmailAction::get_Server


## -description


<p class="CCE_Message">[This interface is no longer supported. Please use IExecAction with the  powershell <a href="https://msdn.microsoft.com/library/Hh849925(v=WPS.620).aspx">Send-MailMessage</a> cmdlet as a workaround.]

Gets or sets the name of the SMTP server that you use to send email from.

This property is read/write.


## -parameters


## -remarks



Make sure the SMTP server that sends the email is setup correctly. E-mail is sent using NTLM authentication for Windows SMTP servers, which means that the security credentials used for running the task must also have privileges on the SMTP server to send email message. If the SMTP server is a non-Windows based server, then the email will be sent if the server allows anonymous access.  For information about setting up the SMTP server, see <a href="http://go.microsoft.com/fwlink/p/?linkid=69001">SMTP Server Setup</a>, and for information about managing SMTP server settings, see <a href="http://go.microsoft.com/fwlink/p/?linkid=69002">SMTP Administration</a>.





## -see-also




<a href="https://msdn.microsoft.com/2f08fd42-233a-40ee-96d0-f0ac8b25b847">IEmailAction</a>
 

 

