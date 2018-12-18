---
UID: NF:mswmdm.IWMDMStorage3.GetMetadata
title: IWMDMStorage3::GetMetadata
author: windows-sdk-content
description: The GetMetadata method retrieves the metadata associated with the storage.
old-location: wmdm\iwmdmstorage3_getmetadata.htm
tech.root: WMDM
ms.assetid: 7e436742-fb19-4e8e-98a2-d961c9f0ecbf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetMetadata, GetMetadata method [windows Media Device Manager], GetMetadata method [windows Media Device Manager],IWMDMStorage3 interface, IWMDMStorage3 interface [windows Media Device Manager],GetMetadata method, IWMDMStorage3.GetMetadata, IWMDMStorage3::GetMetadata, IWMDMStorage3GetMetadata, mswmdm/IWMDMStorage3::GetMetadata, wmdm.iwmdmstorage3_getmetadata
ms.topic: method
req.header: mswmdm.h
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
req.lib: Mssachlp.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mssachlp.lib
 - mssachlp.dll
api_name:
 - IWMDMStorage3.GetMetadata
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDMStorage3::GetMetadata


## -description



The <b>GetMetadata</b> method retrieves the metadata associated with the storage.




## -parameters




### -param ppMetadata [out]

Pointer to an <a href="https://msdn.microsoft.com/ea57a851-0b9f-444c-9819-a278f2ece2b0">IWMDMMetaData</a> pointer associated with a storage. The caller is responsible for calling <b>Release</b> on this interface and all the allocated values when finished with it, as described under "Clearing allocated memory" in <a href="https://msdn.microsoft.com/dd139816-dc8c-4e73-9a21-67287bfe6405">Discovering Device Format Capabilities</a>.


## -returns



The method returns an <b>HRESULT</b>. All the interface methods in Windows Media Device Manager can return any of the following classes of error codes:

<ul>
<li>Standard COM error codes </li>
<li>Windows error codes converted to HRESULT values </li>
<li>Windows Media Device Manager error codes </li>
</ul>
For an extensive list of possible error codes, see <a href="https://msdn.microsoft.com/37e4ad70-afe9-40d6-8c4b-e5fcaa8db4ad">Error Codes</a>.




## -remarks



This method retrieves all metadata associated with the storage. If an application is seeking specific metadata, it might be more efficient to call <a href="https://msdn.microsoft.com/c4e2c889-9ad0-42d1-bb50-4ebcb9859715">IWMDMStorage4::GetSpecifiedMetadata</a>.

When retrieving data from a Windows Portable Devices (WPD) device, the data is returned in binary form. The application should de-serialize this data to obtain the actual property values.


#### Examples

The following C++ function retrieves all the metadata associated with a storage.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>
// Function to print out all the metadata associated with a storage.
HRESULT CWMDMController::GetMetadata(IWMDMStorage *pStorage)
{
   HRESULT hr = S_OK;

   // A dummy loop to handle unrecoverable errors. When we hit an error we
   // can't handle or don't like, we just use a 'break' statement.
   // The custom BREAK_HR macro checks for failed HRESULT values and does this.
   do
   {
      CComPtr&lt;IWMDMStorage3&gt; pStorage3;
      CComPtr&lt;IWMDMMetaData&gt; pMetadata;
      hr = pStorage-&gt;QueryInterface(__uuidof(IWMDMStorage3), (void**)&amp;pStorage3);
      BREAK_HR(hr, "Got an IWMDMStorage3 interface in GetMetadata.", "Couldn't get an IWMDMStorage3 interface in GetMetadata.");

      hr = pStorage3-&gt;GetMetadata(&amp;pMetadata);
      BREAK_HR(hr, "Got an IWMDMMetaData interface in GetMetadata.", "Couldn't get an IWMDMMetaData interface in GetMetadata.");

      //
      // Loop through all metadata properties, and print out the value of each.
      //
      BYTE* value;
      WMDM_TAG_DATATYPE type;
      UINT len = 0;
      UINT count = 0;
      WCHAR* name;
      // Get the number of metadata items.
      hr = pMetadata-&gt;GetItemCount(&amp;count);

      BREAK_HR(hr, "Got a metadata count in GetMetadata.", "Couldn't get a metadata count in GetMetadata.");
      for(;count &gt; 0; count--)
      {
         // Get the metadata property by index.
         WCHAR* name;
         hr = pMetadata-&gt;QueryByIndex(count-1, &amp;name, &amp;type, &amp;value, &amp;len);
         if (SUCCEEDED(hr))
         {
            // TODO: Display the property name.
            CoTaskMemFree(name);

            // Print out the value of the property, according to the value type.
            switch (type)
            {
            case WMDM_TYPE_QWORD:
            case WMDM_TYPE_DWORD:
            case WMDM_TYPE_WORD:
               // TODO: Display the value.
               break;
            case WMDM_TYPE_STRING:
               // TODO: Display the value.
               // Release the method-allocated property value memory.
                    if (SUCCEEDED(hr))
                        CoTaskMemFree(value);
               break;
            case WMDM_TYPE_BOOL:
               // TODO: Display the value.
               break;
            case WMDM_TYPE_BINARY:
               // TODO: Display the value.
               break;
            case WMDM_TYPE_DATE:
               {
                  WMDMDATETIME *val = (WMDMDATETIME*)value;
                        // TODO: Display the month, day, and year.
               }
               break;
            case WMDM_TYPE_GUID:
               {
                  WCHAR strGuid[64];
                  StringFromGUID2(reinterpret_cast&lt;GUID&amp;&gt;(value),(LPOLESTR)strGuid, 64);
                  // TODO: Display the GUID value.
               }
               break;
            default:
               // TODO: Display the message: "Could not understand the returned value type
            }
         }
         else // Couldn't get the metadata property at index count - 1.
            // TODO: Display the message: 
            // "Couldn't get a value for index " 
            // followed by the current index value.
      }

      // Now get a specific property by name.
      // If this property isn't supported, the method returns E_INVALIDARG.
      hr = pMetadata-&gt;QueryByName(g_wszWMDMFileName, &amp;type, &amp;value, &amp;len);
      if (hr == S_OK) 
      {
         wstring wstr((wchar_t*)value, len / 2); // Create a string from the name.
            // TODO: Display the file name.
            CoTaskMemFree(value);
      }

      // See if file is DRM-protected.
      hr = pMetadata-&gt;QueryByName(g_wszWMDMIsProtected, &amp;type, &amp;value, &amp;len);
      if (hr == S_OK)
      {
         // TODO: Display a message that the object is DRM protected.
      }


   }while(FALSE);// End of dummy loop.

   // Clean up and return.
   return hr;
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/ea57a851-0b9f-444c-9819-a278f2ece2b0">IWMDMMetaData Interface</a>



<a href="https://msdn.microsoft.com/b62ea18b-c692-464f-a009-727a2924f8b8">IWMDMStorage3 Interface</a>



<a href="https://msdn.microsoft.com/f06eb965-af34-4247-b8a6-0ac1ee4e4839">IWMDMStorage3::SetMetadata</a>



<a href="https://msdn.microsoft.com/c4e2c889-9ad0-42d1-bb50-4ebcb9859715">IWMDMStorage4::GetSpecifiedMetadata</a>
 

 

