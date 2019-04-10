---
UID: NF:usp10.ScriptItemize
title: ScriptItemize function (usp10.h)
author: windows-sdk-content
description: Breaks a Unicode string into individually shapeable items.
old-location: intl\scriptitemize.htm
tech.root: Intl
ms.assetid: 1491d9c5-e86b-45cc-bb47-85c8619eab69
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ScriptItemize, ScriptItemize function [Internationalization for Windows Applications], _win32_ScriptItemize, intl.scriptitemize, usp10/ScriptItemize
ms.topic: function
req.header: usp10.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Usp10.lib
req.dll: Usp10.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - usp10.dll
 - Ext-MS-Win-usp10-l1-1-0.dll
 - GDI32.dll
 - GDI32Full.dll
api_name:
 - ScriptItemize
product: Windows
targetos: Windows
req.typenames: 
req.redist: Internet Explorer 5 or later on Windows Me/98/95
---

# ScriptItemize function


## -description


Breaks a Unicode string into individually shapeable items.


## -parameters




### -param pwcInChars [in]

Pointer to a Unicode string to itemize.


### -param cInChars [in]

Number of characters in <i>pwcInChars</i> to itemize.


### -param cMaxItems [in]

Maximum number of <a href="https://msdn.microsoft.com/d309f3a7-fec3-4999-bbbe-bb85ceecb4c4">SCRIPT_ITEM</a> structures defining items to process.


### -param psControl [in, optional]

Pointer to a <a href="https://msdn.microsoft.com/4623f606-f67e-48ad-8c1d-d27da5ba556c">SCRIPT_CONTROL</a> structure indicating the type of itemization to perform.

Alternatively, the application can set this parameter to <b>NULL</b> if no <a href="https://msdn.microsoft.com/4623f606-f67e-48ad-8c1d-d27da5ba556c">SCRIPT_CONTROL</a> properties are needed. For more information, see the Remarks section.


### -param psState [in, optional]

Pointer to a <a href="https://msdn.microsoft.com/4b1724f7-7773-42c0-9c19-fbded5aef14e">SCRIPT_STATE</a> structure indicating the initial bidirectional algorithm state.

Alternatively, the application can set this parameter to <b>NULL</b> if the script state is not needed. For more information, see the Remarks section.


### -param pItems [out]

Pointer to a buffer in which the function retrieves <a href="https://msdn.microsoft.com/d309f3a7-fec3-4999-bbbe-bb85ceecb4c4">SCRIPT_ITEM</a> structures representing the items that have been processed. The buffer should be  <code>(cMaxItems + 1) * sizeof(SCRIPT_ITEM)</code> bytes in length. It is invalid to call this function with a buffer to hold less than two <b>SCRIPT_ITEM</b> structures. The function always adds a terminal item to the item analysis array so that the length of the item with zero-based index "i" is always available as:

<code>pItems[i+1].iCharPos - pItems[i].iCharPos;</code>


### -param pcItems [out]

Pointer to the number of <a href="https://msdn.microsoft.com/d309f3a7-fec3-4999-bbbe-bb85ceecb4c4">SCRIPT_ITEM</a> structures processed.


## -returns



Returns 0 if successful. The function returns a nonzero HRESULT value if it does not succeed.

The function returns E_INVALIDARG if <i>pwcInChars</i> is set to <b>NULL</b>, <i>cInChars</i> is 0, <i>pItems</i> is set to <b>NULL</b>, or <i>cMaxItems</i> &lt; 2.

The function returns E_OUTOFMEMORY if the value of <i>cMaxItems</i> is insufficient. As in all error cases, no items are fully processed and no part of the output array contains defined values. If the function returns E_OUTOFMEMORY, the application can call it again with a larger <i>pItems</i> buffer.




## -remarks



See <a href="https://msdn.microsoft.com/e1adc567-0445-4deb-8634-25653f82127c">Displaying Text with Uniscribe</a> for a discussion of the context in which this function is normally called.

The function delimits items by either a change of shaping engine or a change of direction.

The application can create multiple ranges, or runs that fall entirely within a single item, from each <a href="https://msdn.microsoft.com/d309f3a7-fec3-4999-bbbe-bb85ceecb4c4">SCRIPT_ITEM</a> structure retrieved by <b>ScriptItemize</b>. However, it should not combine multiple items into a single run. Later, when measuring or rendering, the application can call <a href="https://msdn.microsoft.com/073ba94a-ebfa-42f5-9d90-d5693dc25703">ScriptShape</a> for each run and must pass the <a href="https://msdn.microsoft.com/c673d5cc-c4ca-4238-8090-55abe3db324b">SCRIPT_ANALYSIS</a> structure retrieved by <b>ScriptItemize</b> in the <a href="https://msdn.microsoft.com/d309f3a7-fec3-4999-bbbe-bb85ceecb4c4">SCRIPT_ITEM</a> structure.

If the text handled by an application can include any right-to-left content, the application uses the <i>psControl</i> and <i>psState</i> parameters in calling <b>ScriptItemize</b>. However, the application does not have to do this and can handle bidirectional text itself instead of relying on Uniscribe to do so. The <i>psControl</i> and <i>psState</i> parameters are useful in some strictly left-to-right scenarios, for example, when the <b>fLinkStringBefore</b> member of <a href="https://msdn.microsoft.com/4623f606-f67e-48ad-8c1d-d27da5ba556c">SCRIPT_CONTROL</a> is not specific to right-to-left scripts. The application sets <i>psControl</i> and <i>psState</i> to <b>NULL</b> to have <b>ScriptItemize</b> break the Unicode string purely by character code.

The application can set all parameters to non-<b>NULL</b> values to have the function perform a full Unicode bidirectional analysis. To permit a correct Unicode bidirectional analysis, the <a href="https://msdn.microsoft.com/4b1724f7-7773-42c0-9c19-fbded5aef14e">SCRIPT_STATE</a> structure should be initialized according to the reading order at paragraph start, and <b>ScriptItemize</b> should be passed the whole paragraph. In particular, the <b>uBidiLevel</b> member should be initialized to 0 for left-to-right and 1 for right-to-left.

The <b>fRTL</b> member of <a href="https://msdn.microsoft.com/c673d5cc-c4ca-4238-8090-55abe3db324b">SCRIPT_ANALYSIS</a> is referenced in <a href="https://msdn.microsoft.com/d309f3a7-fec3-4999-bbbe-bb85ceecb4c4">SCRIPT_ITEM</a> enabled="1". The <b>fNumeric</b> member of <a href="https://msdn.microsoft.com/473c1265-1c2c-48f3-a852-c701bebcf9eb">SCRIPT_PROPERTIES</a> is retrieved by <a href="https://msdn.microsoft.com/4799829d-8122-4bb4-839c-92f177cfd2da">ScriptGetProperties</a>. These members together provide the same classification as the <b>lpClass</b> member of <a href="https://msdn.microsoft.com/7692637e-963a-4e0a-8a04-e05a6d01c417">GCP_RESULTS</a>, referenced by <i>lpResults</i> in <a href="https://msdn.microsoft.com/80d3f4b3-503b-4abb-826c-e5c09972ba2f">GetCharacterPlacement</a>.

European digits U+0030 through U+0039 can be rendered as national digits, as shown in the following table.

<table>
<tr>
<th>SCRIPT_STATE.fDigitSubstitute</th>
<th>SCRIPT_CONTROL.fContextDigits</th>
<th>Digit shapes displayed for Unicode U+0030 through U+0039</th>
</tr>
<tr>
<td><b>FALSE</b></td>
<td>Any</td>
<td>European digits</td>
</tr>
<tr>
<td><b>TRUE</b></td>
<td><b>FALSE</b></td>
<td>As specified in <b>uDefaultLanguage</b> member of <a href="https://msdn.microsoft.com/4623f606-f67e-48ad-8c1d-d27da5ba556c">SCRIPT_CONTROL</a>.</td>
</tr>
<tr>
<td><b>TRUE</b></td>
<td><b>TRUE</b></td>
<td>As prior strong text, defaulting to <b>uDefaultLanguage</b> member of <a href="https://msdn.microsoft.com/4623f606-f67e-48ad-8c1d-d27da5ba556c">SCRIPT_CONTROL</a>.</td>
</tr>
</table>
 

In context digit mode, one of the following actions occurs:

<ul>
<li>If the script specified by <b>uDefaultLanguage</b> is in the same direction as the output, all digits encountered before the first letters are rendered in the language indicated by <b>uDefaultLanguage</b>.</li>
<li>If the script specified by <b>uDefaultLanguage</b> is in the opposite direction from the output, all digits encountered before the first letters are rendered in European digits.</li>
</ul>
For example, if <b>uDefaultLanguage</b> indicates LANG_ARABIC, initial digits are in Arabic-Indic in a right-to-left embedding. However, they are in European digits in a left-to-right embedding.

For more information, see <a href="https://msdn.microsoft.com/6b5267d8-b102-410c-bdc9-831555ca2f84">Digit Shapes</a>.

The Unicode control characters and definitions, and their effects on <a href="https://msdn.microsoft.com/4b1724f7-7773-42c0-9c19-fbded5aef14e">SCRIPT_STATE</a> members, are provided in the following table. For more information on Unicode control characters, see the <a href="http://go.microsoft.com/fwlink/p/?linkid=161649">The Unicode Standard</a>.

<table>
<tr>
<th>Unicode control characters</th>
<th>Meaning</th>
<th>Effect on SCRIPT_STATE</th>
</tr>
<tr>
<td>NADS</td>
<td>Override European digits (NODS) with national digit shapes.</td>
<td>Set <b>fDigitSubstitute</b>.</td>
</tr>
<tr>
<td>NODS</td>
<td>Use nominal digit shapes, otherwise known as European digits. See NADS.</td>
<td>Clear <b>fDigitSubstitute</b>.</td>
</tr>
<tr>
<td>ASS</td>
<td>Activate swapping of symmetric pairs, for example, parentheses. For these characters, left and right are interpreted as opening and closing. This is the default. See ISS.</td>
<td>Clear <b>fInhibitSymSwap</b>.</td>
</tr>
<tr>
<td>ISS</td>
<td>Inhibit swapping of symmetric pairs. See ASS.</td>
<td>Set <b>fInhibitSymSwap</b>.</td>
</tr>
<tr>
<td>AAFS</td>
<td>Activate Arabic form shaping for Arabic presentation forms. See IAFS.</td>
<td>Set <b>fCharShape</b>.</td>
</tr>
<tr>
<td>IAFS</td>
<td>Inhibit Arabic form shaping, that is, ligatures and cursive connections, for Arabic presentation forms. Nominal Arabic characters are not affected. This is the default. See AAFS.</td>
<td>Clear <b>fCharShape</b>.</td>
</tr>
</table>
 

The <b>fArabicNumContext</b> member of <a href="https://msdn.microsoft.com/4b1724f7-7773-42c0-9c19-fbded5aef14e">SCRIPT_STATE</a> supports the context-sensitive display of numerals in Arabic script text. It indicates if digits are rendered using native Arabic script digit shapes or European digits. At the beginning of a paragraph, this member should normally be initialized to <b>TRUE</b> for an Arabic locale, or <b>FALSE</b> for any other locale. The function updates the script state it as it processes strong text.

<div class="alert"><b>Important</b>  Starting with Windows 8: To maintain the ability to run on Windows 7, a module that uses Uniscribe must specify Usp10.lib before gdi32.lib in its library list.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/e1adc567-0445-4deb-8634-25653f82127c">Displaying Text with Uniscribe</a>



<a href="https://msdn.microsoft.com/c673d5cc-c4ca-4238-8090-55abe3db324b">SCRIPT_ANALYSIS</a>



<a href="https://msdn.microsoft.com/4623f606-f67e-48ad-8c1d-d27da5ba556c">SCRIPT_CONTROL</a>



<a href="https://msdn.microsoft.com/d309f3a7-fec3-4999-bbbe-bb85ceecb4c4">SCRIPT_ITEM</a>



<a href="https://msdn.microsoft.com/473c1265-1c2c-48f3-a852-c701bebcf9eb">SCRIPT_PROPERTIES</a>



<a href="https://msdn.microsoft.com/4b1724f7-7773-42c0-9c19-fbded5aef14e">SCRIPT_STATE</a>



<a href="https://msdn.microsoft.com/da15d6b3-6725-43b8-9a2c-c19269a79d1e">ScriptItemizeOpenType</a>



<a href="https://msdn.microsoft.com/073ba94a-ebfa-42f5-9d90-d5693dc25703">ScriptShape</a>



<a href="https://msdn.microsoft.com/de7a882f-ed74-4be2-b66d-59c2e50dc07a">Uniscribe</a>



<a href="https://msdn.microsoft.com/876e36f5-a91c-490b-87bd-b7cb4993f8c4">Uniscribe Functions</a>
 

 

