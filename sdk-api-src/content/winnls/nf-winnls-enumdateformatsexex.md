---
UID: NF:winnls.EnumDateFormatsExEx
title: EnumDateFormatsExEx function (winnls.h)
author: windows-sdk-content
description: Enumerates the long date, short date, or year/month formats that are available for a locale specified by name.Note  The application should call this function in preference to EnumDateFormats or EnumDateFormatsEx if designed to run only on Windows Vista and later. Note  This function can enumerate data that changes between releases, for example, due to a custom locale. If your application must persist or transmit data, see Using Persistent Locale Data.
old-location: intl\enumdateformatsexex.htm
tech.root: Intl
ms.assetid: 52bfec03-4cb3-4418-b467-f75d2900ba40
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DATE_LONGDATE, DATE_MONTHDAY, DATE_SHORTDATE, DATE_YEARMONTH, EnumDateFormatsExEx, EnumDateFormatsExEx function [Internationalization for Windows Applications], _win32_EnumDateFormatsExEx, intl.enumdateformatsexex, winnls/EnumDateFormatsExEx
ms.topic: function
req.header: winnls.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
 - API-MS-Win-Core-Localization-l2-1-0.dll
 - KernelBase.dll
api_name:
 - EnumDateFormatsExEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# EnumDateFormatsExEx function


## -description


Enumerates the long date, short date, or year/month formats that are available for a locale specified by name.<div class="alert"><b>Note</b>  The application should call this function in preference to <a href="https://msdn.microsoft.com/77b5e753-aee9-42d8-a0fa-27b065fc3b20">EnumDateFormats</a> or <a href="https://msdn.microsoft.com/523ef50f-722a-48b9-a2ce-20786b7c79e1">EnumDateFormatsEx</a> if designed to run only on Windows Vista and later.</div>
<div> </div>
<div class="alert"><b>Note</b>  This function can enumerate data that changes between releases, for example, due to a custom locale. If your application must persist or transmit data, see <a href="https://msdn.microsoft.com/f62402d6-31de-4ff7-9538-7925a007a089">Using Persistent Locale Data</a>.</div>
<div> </div>



## -parameters




### -param lpDateFmtEnumProcExEx [in]

Pointer to an application-defined callback function. For more information, see <a href="https://msdn.microsoft.com/ae50e777-4860-4c64-b7c1-debd2048694c">EnumDateFormatsProcExEx</a>.


### -param lpLocaleName [in, optional]

Pointer to a <a href="https://msdn.microsoft.com/221aae7b-3a7c-4995-ae78-50d97de436d8">locale name</a>, or one of the following predefined values. 

<ul>
<li>
<a href="https://msdn.microsoft.com/63e2e368-af2f-4af0-bbea-2b27d1939394">LOCALE_NAME_INVARIANT</a>
</li>
<li>
<a href="https://msdn.microsoft.com/63e2e368-af2f-4af0-bbea-2b27d1939394">LOCALE_NAME_SYSTEM_DEFAULT</a>
</li>
<li>
<a href="https://msdn.microsoft.com/63e2e368-af2f-4af0-bbea-2b27d1939394">LOCALE_NAME_USER_DEFAULT</a>
</li>
</ul>

### -param dwFlags [in]

Flag specifying date formats. The application can supply one of the following values or the <a href="https://msdn.microsoft.com/686ca9f2-515d-449f-8871-77c78ab5c31a">LOCALE_USE_CP_ACP</a> constant.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="DATE_SHORTDATE"></a><a id="date_shortdate"></a><dl>
<dt><b>DATE_SHORTDATE</b></dt>
</dl>
</td>
<td width="60%">
Use short date formats. This value cannot be used with any of the other flag values.

</td>
</tr>
<tr>
<td width="40%"><a id="DATE_LONGDATE"></a><a id="date_longdate"></a><dl>
<dt><b>DATE_LONGDATE</b></dt>
</dl>
</td>
<td width="60%">
Use long date formats. This value cannot be used with any of the other flag values.

</td>
</tr>
<tr>
<td width="40%"><a id="DATE_YEARMONTH"></a><a id="date_yearmonth"></a><dl>
<dt><b>DATE_YEARMONTH</b></dt>
</dl>
</td>
<td width="60%">
Use year/month formats. This value cannot be used with any of the other flag values.

</td>
</tr>
<tr>
<td width="40%"><a id="DATE_MONTHDAY"></a><a id="date_monthday"></a><dl>
<dt><b>DATE_MONTHDAY</b></dt>
</dl>
</td>
<td width="60%">
Use month/day formats. This value cannot be used with any of the other flag values.

</td>
</tr>
</table>
 


### -param lParam [in]

An application-provided parameter to pass to the callback function. This value is especially useful for multi-threaded applications.


## -returns



Returns a nonzero value if successful, or 0 otherwise. To get extended error information, the application can call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>, which can return one of the following error codes:

<ul>
<li>ERROR_BADDB. The function could not access the data. This situation should not normally occur, and typically indicates a bad installation, a disk problem, or the like.</li>
<li>ERROR_INVALID_FLAGS. The values supplied for flags were not valid.</li>
<li>ERROR_INVALID_PARAMETER. Any of the parameter values was invalid.</li>
</ul>



## -remarks



<div class="alert"><b>Note</b>  This API is being updated to support the May 2019 Japanese era change. If your application supports the Japanese calendar, you should validate that it properly handles the new era. See <a href="https://aka.ms/AA3dzcz">Prepare your application for the Japanese era change</a> for more information.</div>
<div> </div>
The function enumerates the date formats by passing date format string pointers, one at a time, to the specified application-defined callback function, along with an application-defined constant that is useful for multi-threaded applications. This process continues until <b>EnumDateFormatsExEx</b> finds the last date format or the callback function returns <b>FALSE</b>.

<b>Beginning in Windows 8:</b> If your app passes language tags to this function from the <a href="https://msdn.microsoft.com/e9e566c3-e84a-44d3-980f-fe8bbd5e052a">Windows.Globalization</a> namespace, it must first convert the tags by calling <a href="https://msdn.microsoft.com/99264b22-3fb5-47e2-b0b9-42a6768e67c1">ResolveLocaleName</a>.




## -see-also




<a href="https://msdn.microsoft.com/77b5e753-aee9-42d8-a0fa-27b065fc3b20">EnumDateFormats</a>



<a href="https://msdn.microsoft.com/523ef50f-722a-48b9-a2ce-20786b7c79e1">EnumDateFormatsEx</a>



<a href="https://msdn.microsoft.com/ae50e777-4860-4c64-b7c1-debd2048694c">EnumDateFormatsProcExEx</a>



<a href="https://msdn.microsoft.com/7a548074-0782-45e1-8051-80c3b9d81885">National Language Support</a>



<a href="https://msdn.microsoft.com/7c72c4de-83be-4b7e-9ed8-b0236c1df8a4">National Language Support Functions</a>
 

 

