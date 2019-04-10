---
UID: NF:wmp.IWMPClosedCaption.put_SAMIStyle
title: IWMPClosedCaption::put_SAMIStyle (wmp.h)
author: windows-sdk-content
description: The put_SAMIStyle method specifies the closed captioning style.
old-location: wmp\iwmpclosedcaption_put_samistyle.htm
tech.root: WMP
ms.assetid: 8f9a4f6e-4596-4c4a-ade7-5b7e1b82b229
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWMPClosedCaption interface [Windows Media Player],put_SAMIStyle method, IWMPClosedCaption.put_SAMIStyle, IWMPClosedCaption::put_SAMIStyle, IWMPClosedCaptionput_SAMIStyle, put_SAMIStyle, put_SAMIStyle method [Windows Media Player], put_SAMIStyle method [Windows Media Player],IWMPClosedCaption interface, wmp.iwmpclosedcaption_put_samistyle, wmp/IWMPClosedCaption::put_SAMIStyle
ms.topic: method
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 9 Series or later.
req.target-min-winversvr: 
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
req.dll: Wmp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmp.dll
api_name:
 - IWMPClosedCaption.put_SAMIStyle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPClosedCaption::put_SAMIStyle


## -description



The <b>put_SAMIStyle</b> method specifies the closed captioning style.




## -parameters




### -param bstrSAMIStyle [in]

<b>BSTR</b> containing the SAMI style.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



A SAMI file can contain several format style definitions. SAMI styles are defined between the &lt;STYLE&gt; and &lt;/STYLE&gt; tags in the SAMI file. A style is defined with a text string preceded by a # character. For example, the following code specifies text formatting to be used for a style.


```

#Emphasis1 {Name: Big Bold Italic; font-size: 14pt; text-align: center;
            color: blue; font-family: sans-serif; font-weight: bold;
            font-style: italic;}


```


If no SAMI style is specified, the first style defined in the SAMI file is used by default.

<b>Windows Media Player 10 Mobile: </b>This method always returns E_INVALIDARG.




## -see-also




<a href="https://msdn.microsoft.com/0fdd2cdc-32d4-4fda-9596-b050107abd5f">Adding Closed Captions to Digital Media</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563113(v=VS.85).aspx">IWMPClosedCaption Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd563124(v=VS.85).aspx">IWMPClosedCaption::get_SAMIStyle</a>
 

 

