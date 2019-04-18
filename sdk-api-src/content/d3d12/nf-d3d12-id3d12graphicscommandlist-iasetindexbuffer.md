---
UID: NF:d3d12.ID3D12GraphicsCommandList.IASetIndexBuffer
title: ID3D12GraphicsCommandList::IASetIndexBuffer (d3d12.h)
author: windows-sdk-content
description: Sets the view for the index buffer.
old-location: direct3d12\id3d12graphicscommandlist_iasetindexbuffer.htm
tech.root: direct3d12
ms.assetid: EB776EC7-42F2-47D3-A1FA-771EC6C4E3AB
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IASetIndexBuffer, IASetIndexBuffer method, IASetIndexBuffer method,ID3D12GraphicsCommandList interface, ID3D12GraphicsCommandList interface,IASetIndexBuffer method, ID3D12GraphicsCommandList.IASetIndexBuffer, ID3D12GraphicsCommandList::IASetIndexBuffer, d3d12/ID3D12GraphicsCommandList::IASetIndexBuffer, direct3d12.id3d12graphicscommandlist_iasetindexbuffer
ms.topic: method
req.header: d3d12.h
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
req.lib: D3d12.lib
req.dll: D3d12.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - d3d12.dll
api_name:
 - ID3D12GraphicsCommandList.IASetIndexBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D12GraphicsCommandList::IASetIndexBuffer


## -description


Sets the view for the index buffer.
        


## -parameters




### -param pView [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/CADD98BF-EDA9-43D6-9ADA-392051541B61">D3D12_INDEX_BUFFER_VIEW</a>*</b>

The view specifies the index buffer's address, size, and <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>, as a pointer to a <a href="https://msdn.microsoft.com/CADD98BF-EDA9-43D6-9ADA-392051541B61">D3D12_INDEX_BUFFER_VIEW</a> structure.
          


## -returns



This method does not return a value.
          




## -remarks



Only one index buffer can be bound to the graphics pipeline at any one time.


#### Examples

The <a href="https://msdn.microsoft.com/4C4475D4-534F-484F-8D60-9ACEA09AC109">D3D12Bundles</a> sample uses <b>ID3D12GraphicsCommandList::IASetIndexBuffer</b> as follows:
        


```cpp
void FrameResource::PopulateCommandList(ID3D12GraphicsCommandList* pCommandList, ID3D12PipelineState* pPso1, ID3D12PipelineState* pPso2,
    UINT frameResourceIndex, UINT numIndices, D3D12_INDEX_BUFFER_VIEW* pIndexBufferViewDesc, D3D12_VERTEX_BUFFER_VIEW* pVertexBufferViewDesc,
    ID3D12DescriptorHeap* pCbvSrvDescriptorHeap, UINT cbvSrvDescriptorSize, ID3D12DescriptorHeap* pSamplerDescriptorHeap, ID3D12RootSignature* pRootSignature)
{
    // If the root signature matches the root signature of the caller, then
    // bindings are inherited, otherwise the bind space is reset.
    pCommandList->SetGraphicsRootSignature(pRootSignature);

    ID3D12DescriptorHeap* ppHeaps[] = { pCbvSrvDescriptorHeap, pSamplerDescriptorHeap };
    pCommandList->SetDescriptorHeaps(_countof(ppHeaps), ppHeaps);
    pCommandList->IASetPrimitiveTopology(D3D_PRIMITIVE_TOPOLOGY_TRIANGLELIST);

    pCommandList->IASetIndexBuffer(pIndexBufferViewDesc);

    pCommandList->IASetVertexBuffers(0, 1, pVertexBufferViewDesc);

    pCommandList->SetGraphicsRootDescriptorTable(0, pCbvSrvDescriptorHeap->GetGPUDescriptorHandleForHeapStart());
    pCommandList->SetGraphicsRootDescriptorTable(1, pSamplerDescriptorHeap->GetGPUDescriptorHandleForHeapStart());

    // Calculate the descriptor offset due to multiple frame resources.
    // 1 SRV + how many CBVs we have currently.
    UINT frameResourceDescriptorOffset = 1 + (frameResourceIndex * m_cityRowCount * m_cityColumnCount);
    CD3DX12_GPU_DESCRIPTOR_HANDLE cbvSrvHandle(pCbvSrvDescriptorHeap->GetGPUDescriptorHandleForHeapStart(), frameResourceDescriptorOffset, cbvSrvDescriptorSize);

    BOOL usePso1 = TRUE;
    for (UINT i = 0; i < m_cityRowCount; i++)
    {
        for (UINT j = 0; j < m_cityColumnCount; j++)
        {
            // Alternate which PSO to use; the pixel shader is different on 
            // each just as a PSO setting demonstration.
            pCommandList->SetPipelineState(usePso1 ? pPso1 : pPso2);
            usePso1 = !usePso1;

            // Set this city's CBV table and move to the next descriptor.
            pCommandList->SetGraphicsRootDescriptorTable(2, cbvSrvHandle);
            cbvSrvHandle.Offset(cbvSrvDescriptorSize);

            pCommandList->DrawIndexedInstanced(numIndices, 1, 0, 0, 0);
        }
    }
}

```


See <a href="https://msdn.microsoft.com/C2323482-D06D-43B7-9BDE-BFB9A6A6B70D">Example Code in the D3D12 Reference</a>.
        

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/1BF282A7-F6D4-43A9-BDAD-D877564A1C6B">ID3D12GraphicsCommandList</a>
 

 

