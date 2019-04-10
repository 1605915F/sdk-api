---
UID: NN:d3d11.ID3D11VideoContext
title: ID3D11VideoContext (d3d11.h)
author: windows-sdk-content
description: Provides the video functionality of a Microsoft Direct3D 11 device.
old-location: mf\id3d11videocontext.htm
tech.root: medfound
ms.assetid: 6EF09C31-56C7-46B5-87AE-B1FE43EC66FC
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ID3D11VideoContext, ID3D11VideoContext interface [Media Foundation], ID3D11VideoContext interface [Media Foundation],described, d3d11/ID3D11VideoContext, mf.id3d11videocontext
ms.topic: interface
req.header: d3d11.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
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
 - COM
api_location:
 - d3d11.h
api_name:
 - ID3D11VideoContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11VideoContext interface


## -description


Provides the video functionality of a Microsoft Direct3D 11 device. 


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ID3D11VideoContext</b> interface inherits from <a href="https://msdn.microsoft.com/bed17239-0358-4768-8655-9a1d92f25a2e">ID3D11DeviceChild</a>. <b>ID3D11VideoContext</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ID3D11VideoContext</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6564EC13-A7B3-4A48-8776-4CD46BFF8E8F">ConfigureAuthenticatedChannel</a>
</td>
<td align="left" width="63%">
Sends a configuration command to an authenticated channel.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/395B06D8-1BCF-44F2-9F69-A183C30E36B7">DecoderBeginFrame</a>
</td>
<td align="left" width="63%">
Starts a decoding operation to decode a video frame.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/3596B70C-4BED-49C4-A0E4-8702DA219B01">DecoderEndFrame</a>
</td>
<td align="left" width="63%">
Signals the end of a decoding operation.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/B96FD793-C82A-4752-8F59-3CC9B86D1C2D">DecoderExtension</a>
</td>
<td align="left" width="63%">
Performs an extended function for decoding.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E693D97A-E21F-4133-B56A-490F92CBD945">DecryptionBlt</a>
</td>
<td align="left" width="63%">
Writes encrypted data to a protected surface.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2BBD0BC2-53D9-435E-835C-20A992118329">EncryptionBlt</a>
</td>
<td align="left" width="63%">
Reads encrypted data from a protected surface.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2F602A5E-B5D1-4749-8696-9F0594770B4F">FinishSessionKeyRefresh</a>
</td>
<td align="left" width="63%">
Switches to a new session key.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6842D5D7-6165-4428-91BD-2234BE5332B8">GetDecoderBuffer</a>
</td>
<td align="left" width="63%">
Gets a pointer to a decoder buffer.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/B62BE7CB-75FA-45E9-9AB7-83738DFE3B19">GetEncryptionBltKey</a>
</td>
<td align="left" width="63%">
Gets the cryptographic key to decrypt the data returned by the <a href="https://msdn.microsoft.com/2BBD0BC2-53D9-435E-835C-20A992118329">ID3D11VideoContext::EncryptionBlt</a> method.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/FF546AE5-D062-41A9-B143-8B25466BF6E3">NegotiateAuthenticatedChannelKeyExchange</a>
</td>
<td align="left" width="63%">
Establishes a session key for an authenticated channel.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/76160B03-6F7F-4618-859B-0A7E73540CA4">NegotiateCryptoSessionKeyExchange</a>
</td>
<td align="left" width="63%">
Establishes the session key for a cryptographic session.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4E059358-E1FD-4EDB-B1D4-982802385232">QueryAuthenticatedChannel</a>
</td>
<td align="left" width="63%">
Sends a query to an authenticated channel.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/C7BD4CA6-706D-4C3A-AED1-EDF1C65E41E0">ReleaseDecoderBuffer</a>
</td>
<td align="left" width="63%">
Releases a buffer that was obtained by calling the <a href="https://msdn.microsoft.com/6842D5D7-6165-4428-91BD-2234BE5332B8">ID3D11VideoContext::GetDecoderBuffer</a> method.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/63376BFE-BA84-4268-8AA8-128BEB83AE78">StartSessionKeyRefresh</a>
</td>
<td align="left" width="63%">
Gets a random number that can be used to refresh the session key.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/39010E57-FFF2-4793-B839-E336E8D2C1B2">SubmitDecoderBuffers</a>
</td>
<td align="left" width="63%">
Submits one or more buffers for decoding.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/D526BB31-A4B9-4BBD-BAE3-43FDFF58A32A">VideoProcessorBlt</a>
</td>
<td align="left" width="63%">
Performs a video processing operation on one or more input samples and writes the result to a Direct3D surface.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/23F37D9C-3D33-4A07-AC54-5273A09BF540">VideoProcessorGetOutputAlphaFillMode</a>
</td>
<td align="left" width="63%">
Gets the current alpha fill mode for the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/B22666BC-EADF-4812-B299-1EA45F1943C4">VideoProcessorGetOutputBackgroundColor</a>
</td>
<td align="left" width="63%">
Gets the current background color for the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/26D9C908-D8A6-44F9-895F-48C52F4C8B59">VideoProcessorGetOutputColorSpace</a>
</td>
<td align="left" width="63%">
Gets the current output color space for the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/40F7D380-C385-4C1C-90E5-E362CA54CD41">VideoProcessorGetOutputConstriction</a>
</td>
<td align="left" width="63%">
Gets the current level of downsampling that is performed by the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/3B979D5D-CB3D-4B67-9BE3-277005076604">VideoProcessorGetOutputExtension</a>
</td>
<td align="left" width="63%">
Gets private state data from the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E7BDB9DA-2760-416D-BD51-F73A035B790A">VideoProcessorGetOutputStereoMode</a>
</td>
<td align="left" width="63%">
Queries whether the video processor produces stereo video frames.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5D59822A-B322-4E79-A543-A89C2232C62F">VideoProcessorGetOutputTargetRect</a>
</td>
<td align="left" width="63%">
Gets the current target rectangle for the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E2DB0672-54D9-4DDB-B6EA-9935237C33FB">VideoProcessorGetStreamAlpha</a>
</td>
<td align="left" width="63%">
Gets the planar alpha for an input stream on the video processor.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/FD7B20C2-5418-4CA5-A64E-FA84D4070A10">VideoProcessorGetStreamAutoProcessingMode</a>
</td>
<td align="left" width="63%">
Queries whether automatic processing features of the video processor are enabled.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4D66147C-D4FC-40BC-B406-B40B6EA24D94">VideoProcessorGetStreamColorSpace</a>
</td>
<td align="left" width="63%">
Gets the color space for an input stream of the video processor.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/F7968C74-8053-4A16-88C7-30729900B95D">VideoProcessorGetStreamDestRect</a>
</td>
<td align="left" width="63%">
Gets the destination rectangle for an input stream on the video processor.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/33A2DC3D-4B92-45B5-B67A-7F3AA55F061B">VideoProcessorGetStreamExtension</a>
</td>
<td align="left" width="63%">
Gets a driver-specific state for a video processing stream.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E18146E9-FBF4-4A1E-AC6C-7500CDA9DC59">VideoProcessorGetStreamFilter</a>
</td>
<td align="left" width="63%">
Gets the image filter settings for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/43879368-1730-4881-B77E-0A975DD5E473">VideoProcessorGetStreamFrameFormat</a>
</td>
<td align="left" width="63%">
Gets the format of an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1DE22456-84E9-478F-A6CA-4C9CACF7E9AF">VideoProcessorGetStreamLumaKey</a>
</td>
<td align="left" width="63%">
Gets the luma key for an input stream of the video processor.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/69AC0713-FE92-4D89-857A-A0037D51B597">VideoProcessorGetStreamOutputRate</a>
</td>
<td align="left" width="63%">
Gets the rate at which the video processor produces output frames for an input stream.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/009568EA-7230-42C0-B35F-AB0A1AF8EC2A">VideoProcessorGetStreamPalette</a>
</td>
<td align="left" width="63%">
Gets the color-palette entries for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/45B0CF31-6552-4C75-B32F-755398D1A054">VideoProcessorGetStreamPixelAspectRatio</a>
</td>
<td align="left" width="63%">
Gets the pixel aspect ratio for an input stream on the video processor.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6593d829-7f33-408e-aac1-f13e59f7b4bd">VideoProcessorGetStreamRotation</a>
</td>
<td align="left" width="63%">
Gets the stream rotation  for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/52AFE959-695B-4797-ABCF-B8264046E4BE">VideoProcessorGetStreamSourceRect</a>
</td>
<td align="left" width="63%">
Gets the source rectangle for an input stream on the video processor.



</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/FCEE6C95-C631-4268-9B06-686B8AC7D80C">VideoProcessorGetStreamStereoFormat</a>
</td>
<td align="left" width="63%">
Gets the stereo 3D format for an input stream on the video processor

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/898604FA-B857-4D84-AA0D-3BC517F75A36">VideoProcessorSetOutputAlphaFillMode</a>
</td>
<td align="left" width="63%">
Sets the alpha fill mode for data that the video processor writes to the render target.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6D6DAECC-8D20-4ABB-A20B-55EC4F68D8F1">VideoProcessorSetOutputBackgroundColor</a>
</td>
<td align="left" width="63%">
Sets the background color for the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5B4B2C26-CFC8-43BD-A889-8838DEF3582A">VideoProcessorSetOutputColorSpace</a>
</td>
<td align="left" width="63%">
Sets the output color space for the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/EA61A4B8-0853-4F17-B634-70A896DCF5F7">VideoProcessorSetOutputConstriction</a>
</td>
<td align="left" width="63%">
Sets the amount of downsampling to perform on the output.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/38279599-09C8-4BB1-8946-0B066D96E22B">VideoProcessorSetOutputExtension</a>
</td>
<td align="left" width="63%">
Sets a driver-specific video processing state.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/86449010-6F46-460B-9972-4186FD84B407">VideoProcessorSetOutputStereoMode</a>
</td>
<td align="left" width="63%">
Specifies whether the video processor produces stereo video frames.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/D49EED28-E26E-48B5-A050-8EB568A3D31A">VideoProcessorSetOutputTargetRect</a>
</td>
<td align="left" width="63%">
Sets the target rectangle for the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/DA869E3F-25BB-4794-B7AE-A3C2DA968800">VideoProcessorSetStreamAlpha</a>
</td>
<td align="left" width="63%">
Sets the planar alpha for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/92579A03-AA8A-4D9B-8150-F5FDDBAFC1C1">VideoProcessorSetStreamAutoProcessingMode</a>
</td>
<td align="left" width="63%">
Enables or disables automatic processing features on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/EFF6BF9B-CC96-4D57-A97A-B3E8457346B5">VideoProcessorSetStreamColorSpace</a>
</td>
<td align="left" width="63%">
Sets the color space for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/F3C77812-9096-4D65-9D6C-082133C873A7">VideoProcessorSetStreamDestRect</a>
</td>
<td align="left" width="63%">
Sets the destination rectangle for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E6E1CF26-6A9F-42E1-8DA7-2AC76CE05906">VideoProcessorSetStreamExtension</a>
</td>
<td align="left" width="63%">
Sets a driver-specific state on a video processing stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/49258E8F-50BC-4F51-A492-78B44A73CC13">VideoProcessorSetStreamFilter</a>
</td>
<td align="left" width="63%">
Enables or disables an image filter for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/248BE244-23A9-4F4E-95F7-D3DB678B2D9F">VideoProcessorSetStreamFrameFormat</a>
</td>
<td align="left" width="63%">
Specifies whether an input stream on the video processor contains interlaced or progressive frames.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/DAFDAF7C-BBE2-41AA-9E44-C1BD28CE03FE">VideoProcessorSetStreamLumaKey</a>
</td>
<td align="left" width="63%">
Sets the luma key for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/D353F6E8-B465-46CB-AA47-8B097AB4AF2A">VideoProcessorSetStreamOutputRate</a>
</td>
<td align="left" width="63%">
Sets the rate at which the video processor produces output frames for an input stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/E2816D5F-0541-45B0-A90A-7C26530D064C">VideoProcessorSetStreamPalette</a>
</td>
<td align="left" width="63%">
Sets the color-palette entries for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4205F6F0-4AF3-42B1-8636-64FCFC865856">VideoProcessorSetStreamPixelAspectRatio</a>
</td>
<td align="left" width="63%">
Sets the pixel aspect ratio for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/f94d283c-5eea-4248-8c06-46ef66e86b22">VideoProcessorSetStreamRotation</a>
</td>
<td align="left" width="63%">
Sets the stream rotation for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/A2771C8A-13AB-4AFA-87A1-1390B582342A">VideoProcessorSetStreamSourceRect</a>
</td>
<td align="left" width="63%">
Sets the source rectangle for an input stream on the video processor.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/FAAE902A-622E-42D2-B332-CD4126A4182E">VideoProcessorSetStreamStereoFormat</a>
</td>
<td align="left" width="63%">
Enables or disables stereo 3D video for an input stream on the video processor.

</td>
</tr>
</table> 


## -remarks



To get a pointer to this interface, call <a href="https://msdn.microsoft.com/54d5ff80-18db-43f2-b636-f93ac053146d">QueryInterface</a> with an <a href="https://msdn.microsoft.com/afb32c09-77f2-4c33-bd93-8dce92a2e45e">ID3D11DeviceContext</a> interface pointer.

This interface provides access to several areas of Microsoft Direct3Dvideo functionality:

<ul>
<li>Hardware-accelerated video decoding</li>
<li>Video processing</li>
<li>GPU-based content protection</li>
<li>Video encryption and decryption</li>
</ul>
In Microsoft Direct3D 9, the equivalent functions were distributed across several interfaces:

<ul>
<li>
<a href="https://msdn.microsoft.com/dd969956-a140-44ed-9917-5a0a09a432fa">IDirect3DAuthenticatedChannel9</a>
</li>
<li>
<a href="https://msdn.microsoft.com/2511c9da-e696-4e49-b180-7fc1317c1652">IDirect3DCryptoSession9</a>
</li>
<li>
<a href="https://msdn.microsoft.com/116c19a3-39be-4f96-969f-f3d62ed33a70">IDirectXVideoDecoder</a>
</li>
<li>
<a href="https://msdn.microsoft.com/a9bc3162-4f37-4f0b-8a8e-8ebeb8f0d8d5">IDirectXVideoProcessor</a>
</li>
<li>
<a href="https://msdn.microsoft.com/cbfacff5-1cbb-4296-8242-c06b43fc95af">IDXVAHD_VideoProcessor</a>
</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/2AE97FFE-0FA4-4CC0-8433-7BA46BCACE30">Direct3D 11 Video Interfaces</a>



<a href="https://msdn.microsoft.com/bed17239-0358-4768-8655-9a1d92f25a2e">ID3D11DeviceChild</a>



<a href="https://msdn.microsoft.com/64D12F68-C2AA-4C1D-9608-5F97CF7AD430">ID3D11VideoContext1</a>
 

 

