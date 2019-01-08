---
UID: NC:commctrl.PFTASKDIALOGCALLBACK
title: PFTASKDIALOGCALLBACK
author: windows-sdk-content
description: The TaskDialogCallbackProc function is an application-defined function used with the TaskDialogIndirect function.
old-location: controls\TaskDialogCallbackProc.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\taskdialogs\taskdialogreference\taskdialogfunctions\taskdialogcallbackproc.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PFTASKDIALOGCALLBACK, PFTASKDIALOGCALLBACK callback, PFTASKDIALOGCALLBACK callback function [Windows Controls], _shell_TaskDialogCallbackProc, _shell_TaskDialogCallbackProc_cpp, commctrl/PFTASKDIALOGCALLBACK, controls.TaskDialogCallbackProc, controls._shell_TaskDialogCallbackProc
ms.topic: callback
req.header: commctrl.h
req.include-header: Commctrl.h
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
 - UserDefined
api_location:
 - Commctrl.h
api_name:
 - PFTASKDIALOGCALLBACK
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PFTASKDIALOGCALLBACK callback function


## -description


The <i>TaskDialogCallbackProc</i> function is an application-defined function used with the <a href="https://msdn.microsoft.com/en-us/library/Bb760544(v=VS.85).aspx">TaskDialogIndirect</a> function. It receives messages from the task dialog when various events occur.

The <b>PFTASKDIALOGCALLBACK</b> type defines a pointer to this callback function. <i>TaskDialogCallbackProc</i> is a placeholder for the application defined function name.


## -parameters




### -param hwnd [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the TaskDialog window. Do not continue sending messages to hwnd after the callback procedure returns from having been called with <a href="https://msdn.microsoft.com/en-us/library/Bb787483(v=VS.85).aspx">TDN_DESTROYED</a>.
				


### -param msg


### -param wParam [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">WPARAM</a></b>

Specifies additional notification information.  The contents of this parameter depend on the value of the <i>uNotification</i> parameter.


### -param lParam [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPARAM</a></b>

Specifies additional notification information.  The contents of this parameter depend on the value of the <i>uNotification</i> parameter.


### -param lpRefData








#### - dwRefData [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG_PTR</a></b>

Pointer to application specific data. This is the data pointed to by the <b>lpCallbackData</b> member of structure <a href="https://msdn.microsoft.com/en-us/library/Bb787473(v=VS.85).aspx">TASKDIALOGCONFIG</a> used to create the task dialog.


#### - uNotification [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

One of the following notifications.
				

<table class="clsStd">
<tr>
<th>Notification</th>
<th>Usage</th>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787477(v=VS.85).aspx">TDN_BUTTON_CLICKED</a>
</td>
<td>Indicates that a button has been selected. The command ID of the button is specified by <i>wParam</i>.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787479(v=VS.85).aspx">TDN_CREATED</a>
</td>
<td>Indicates that the Task Dialog has been created.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787483(v=VS.85).aspx">TDN_DESTROYED</a>
</td>
<td>Indicates that the Task Dialog has been destroyed.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787485(v=VS.85).aspx">TDN_DIALOG_CONSTRUCTED</a>
</td>
<td>Indicates that the Task Dialog has been created but has not been displayed yet.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787487(v=VS.85).aspx">TDN_EXPANDO_BUTTON_CLICKED</a>
</td>
<td>Indicates that the exando button has been selected.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787489(v=VS.85).aspx">TDN_HELP</a>
</td>
<td>Indicates that the F1 key has been pressed while the Task Dialog has focus.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787491(v=VS.85).aspx">TDN_HYPERLINK_CLICKED</a>
</td>
<td>Indicates that a hyperlink has been selected. A pointer to the link text is specified by <i>lParam</i>.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787492(v=VS.85).aspx">TDN_NAVIGATED</a>
</td>
<td>Indicates that navigation has occurred.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787494(v=VS.85).aspx">TDN_RADIO_BUTTON_CLICKED</a>
</td>
<td>Indicates that a radio button has been selected. The command ID of the radio button is specified by <i>wParam</i>.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787481(v=VS.85).aspx">TDN_TIMER</a>
</td>
<td>Indicates that the Task Dialog timer has fired. The total elapsed time is specified by <i>wParam</i>. You can update the progress bar by sending a <a href="https://msdn.microsoft.com/en-us/library/Bb760530(v=VS.85).aspx">TDM_SET_PROGRESS_BAR_POS</a> message to the window specified by the <i>hwnd</i> parameter.</td>
</tr>
<tr>
<td>
<a href="https://msdn.microsoft.com/en-us/library/Bb787497(v=VS.85).aspx">TDN_VERIFICATION_CLICKED</a>
</td>
<td>Indicates that the Task Dialog verification check box has been selected.</td>
</tr>
</table>
 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

The return value is specific to the notification being processed. When responding to a button click, your implementation should return S_FALSE if the Task Dialog is not to close. Otherwise return S_OK.




## -remarks



An application must register this callback function by passing its address in the <b>pfCallback</b> member of  the <a href="https://msdn.microsoft.com/en-us/library/Bb787473(v=VS.85).aspx">TASKDIALOGCONFIG</a> structure that is passed via pointer through <a href="https://msdn.microsoft.com/en-us/library/Bb760544(v=VS.85).aspx">TaskDialogIndirect</a>.



