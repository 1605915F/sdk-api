---
UID: NF:d2d1.ID2D1RenderTarget.FillRoundedRectangle
title: ID2D1RenderTarget::FillRoundedRectangle
author: windows-sdk-content
description: Paints the interior of the specified rounded rectangle.
old-location: direct2d\id2d1rendertarget_fillroundedrectangle.htm
tech.root: Direct2D
ms.assetid: 9c4765b0-858f-4a20-b044-0acf87a1f131
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FillRoundedRectangle, FillRoundedRectangle methods [Direct2D], ID2D1RenderTarget.FillRoundedRectangle, ID2D1RenderTarget::FillRoundedRectangle, d2d1/FillRoundedRectangle, direct2d.id2d1rendertarget_fillroundedrectangle
ms.topic: method
req.header: d2d1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
req.lib: D2d1.lib
req.dll: D2d1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - D2d1.dll
api_name:
 - ID2D1RenderTarget::FillRoundedRectangle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1RenderTarget::FillRoundedRectangle


## -description


<span>Paints the interior of the specified rounded rectangle.
</span><h3>Overload list</h3><table>
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr>
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/db000907-eff2-4cf7-a805-be1ff4cb30fe">FillRoundedRectangle(D2D1_ROUNDED_RECT&,ID2D1Brush*)</a>
</td>
<td align="left" width="63%">
Paints the interior of the specified rounded rectangle.

</td>
</tr>
<tr>
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/421ddc6a-faf6-494b-8c22-6df83e6541ae">FillRoundedRectangle(D2D1_ROUNDED_RECT*,ID2D1Brush*)</a>
</td>
<td align="left" width="63%">
Paints the interior of the specified rounded rectangle.

</td>
</tr>
</table>

## -parameters


## -remarks



This method doesn't return an error code if it fails. To determine whether a drawing operation (such as <b>FillRoundedRectangle</b>) failed, check the result returned by the <a href="https://msdn.microsoft.com/a8f24501-4e85-4981-bb38-2bd6333a7b49">ID2D1RenderTarget::EndDraw</a> or <a href="https://msdn.microsoft.com/3ad9c966-85f5-4ddb-a8c1-aefcba533509">ID2D1RenderTarget::Flush</a> methods. 


#### Examples

The following example uses the <a href="https://msdn.microsoft.com/en-us/library/Dd742847(v=VS.85).aspx">DrawRoundedRectangle</a> and <b>FillRoundedRectangle</b> methods to outline and fill a rounded rectangle.  This example produces the output shown in the following illustration.

<img alt="Illustration of four rounded rectangles with different stroke styles and fills" src="images/drawroundedrectangle_scr.png"/>

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>//  Called whenever the application needs to display the client
//  window.
HRESULT DrawAndFillRoundedRectangleExample::OnRender()
{
    HRESULT hr;

    // Create the render target and brushes if they
    // don't already exists.
    hr = CreateDeviceResources();

    if (SUCCEEDED(hr))
    {
        // Retrieve the size of the render target.
        D2D1_SIZE_F renderTargetSize = m_pRenderTarget-&gt;GetSize();

        m_pRenderTarget-&gt;BeginDraw();
        m_pRenderTarget-&gt;SetTransform(D2D1::Matrix3x2F::Identity());
        m_pRenderTarget-&gt;Clear(D2D1::ColorF(D2D1::ColorF::White));

        // Paint a grid background.
        m_pRenderTarget-&gt;FillRectangle(
            D2D1::RectF(0.0f, 0.0f, renderTargetSize.width, renderTargetSize.height),
            m_pGridPatternBitmapBrush
            );

        // Define a rounded rectangle.
        D2D1_ROUNDED_RECT roundedRect = D2D1::RoundedRect(
            D2D1::RectF(20.f, 20.f, 150.f, 100.f),
            10.f,
            10.f
            );

        // Draw the rectangle.
        m_pRenderTarget-&gt;DrawRoundedRectangle(roundedRect, m_pBlackBrush, 10.f);

        // Apply a translation transform.
        m_pRenderTarget-&gt;SetTransform(D2D1::Matrix3x2F::Translation(200.f, 0.f));

        // Draw the rounded rectangle again, this time with a dashed stroke.
        m_pRenderTarget-&gt;DrawRoundedRectangle(roundedRect, m_pBlackBrush, 10.f, m_pStrokeStyle);

        // Apply another translation transform.
        m_pRenderTarget-&gt;SetTransform(D2D1::Matrix3x2F::Translation(0.f, 150.f));

        // Draw, then fill the rounded rectangle.
        m_pRenderTarget-&gt;DrawRoundedRectangle(roundedRect, m_pBlackBrush, 10.f, m_pStrokeStyle);
        m_pRenderTarget-&gt;FillRoundedRectangle(roundedRect, m_pSilverBrush);

        // Apply another translation transform.
        m_pRenderTarget-&gt;SetTransform(D2D1::Matrix3x2F::Translation(200.f, 150.f));

        // Fill, then draw the rounded rectangle.
        m_pRenderTarget-&gt;FillRoundedRectangle(roundedRect, m_pSilverBrush);
        m_pRenderTarget-&gt;DrawRoundedRectangle(roundedRect, m_pBlackBrush, 10.f, m_pStrokeStyle);

        hr = m_pRenderTarget-&gt;EndDraw();

        if (hr == D2DERR_RECREATE_TARGET)
        {
            hr = S_OK;
            DiscardDeviceResources();
        }
    }

    return hr;
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/200119a2-941c-493f-9e56-c9f306dc5322">D2D1::RoundedRect</a>



<a href="https://msdn.microsoft.com/8a68fc3f-118c-447b-856c-05417ae4ef29">How to Draw and Fill a Basic Shape</a>



<a href="https://msdn.microsoft.com/40629be9-5840-4bde-b369-56bbfd791775">ID2D1RenderTarget</a>
 

 

