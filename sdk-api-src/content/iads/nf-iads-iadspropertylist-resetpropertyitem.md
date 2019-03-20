---
UID: NF:iads.IADsPropertyList.ResetPropertyItem
title: IADsPropertyList::ResetPropertyItem (iads.h)
author: windows-sdk-content
description: Removes the specified item from the list; that is, from the cache.
old-location: adsi\iadspropertylist_resetpropertyitem.htm
tech.root: adsi
ms.assetid: 25ee4444-476d-4146-ac22-3b0cfed3f2c0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IADsPropertyList interface [ADSI],ResetPropertyItem method, IADsPropertyList.ResetPropertyItem, IADsPropertyList::ResetPropertyItem, ResetPropertyItem, ResetPropertyItem method [ADSI], ResetPropertyItem method [ADSI],IADsPropertyList interface, _ds_iadspropertylist_resetpropertyitem, adsi.iadspropertylist__resetpropertyitem, adsi.iadspropertylist_resetpropertyitem, iads/IADsPropertyList::ResetPropertyItem
ms.topic: method
req.header: iads.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: Activeds.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Activeds.dll
api_name:
 - IADsPropertyList.ResetPropertyItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IADsPropertyList::ResetPropertyItem


## -description


The <b>IADsPropertyList::ResetPropertyItem</b> method removes the specified item from the list; that is, from the cache. You can specify the item to be removed by name (as a string) or by index (as an integer).


## -parameters




### -param varEntry [in]

Entry to be reset.


## -returns



This method supports the standard <b>HRESULT</b> return values, including <b>S_OK</b>. For more information and other return values, see  <a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>.




## -remarks



<b>ResetPropertyItem</b> only affects the contents of the cache and does not affect the properties on the actual object in the directory; that is calling  <a href="https://msdn.microsoft.com/e7ff6acd-b7c4-463d-a34f-fd793067c63a">SetInfo</a> after calling <b>ResetPropertyItem</b> does not delete the properties on the directory object.


#### Examples

The following code example shows how to implement <b>ResetPropertyItem</b>.


```vb
Dim propList As IADsPropertyList

On Error GoTo Cleanup
 
Set propList = GetObject("LDAP://DC=Fabrikam,DC=com")
 
'--- Now modify the cache using PutPropertyItem
Set propVal = New PropertyValue
'--- Property Value-----
propVal.CaseIgnoreString = "Fabrikam"
propVal.ADsType = ADSTYPE_CASE_IGNORE_STRING
 
'--- Property Entry ----
Set propEntry = New PropertyEntry
propEntry.Name = "adminDescription"
propEntry.Values = Array(propVal)
propEntry.ControlCode = ADS_PROPERTY_UPDATE
propEntry.ADsType = ADS_CASE_IGNORE_STRING
 
' --- Property List----
propList.PutPropertyItem (propEntry)
 
' Commit to the directory. Without this, the changes take place only in the cache.
propList.SetInfo 
 
propList.GetInfo
Debug.Print " Number of Properties = " & propList.PropertyCount
propList.ResetPropertyItem "adminDescription"
 
' the property count should have been reduced by one.
Debug.Print "Number of properties = " & propList.PropertyCount

Cleanup:
    If (Err.Number<>0) Then
        MsgBox("An error has occurred. " & Err.Number)
    End If
    Set propList = Nothing
    Set propVal = Nothing
    Set propEntry = Nothing

```


The following code example shows the effect produced by a call to <b>IADsPropertyList::ResetPropertyItem</b>. For more information and the listing of the <b>GetPropertyCache</b> function, see  <a href="https://msdn.microsoft.com/70e9ce0e-ae83-43b7-8b84-99d5e1f8a8d2">IADsPropertyList</a>. For more information and the listing of the <b>GetNextEntry</b> and <b>PropertyItem</b> functions, see  <a href="https://msdn.microsoft.com/2a12ba88-363b-41e3-bd05-8a71f5317097">IADsPropertyList::Next</a> and  <a href="https://msdn.microsoft.com/6e103872-ea2e-4178-9c8a-b958ae3bcf85">IADsPropertyList::Item</a> respectively.


```cpp
IADsPropertyList *GetPropertyCache(LPWSTR);
IADsPropertyEntry *GetNextEntry(IADsPropertyList *);
IADsPropertyEntry *PropertyItem(IADsPropertyList *,LPWSTR);
 
void ResetItem(IADsPropertyList *pList, LPWSTR item)
{
    VARIANT var;
    VariantInit(&var);

    if(!pList)
    {
        item = NULL;
        return;
    }

    V_BSTR(&var)=SysAllocString(item);
    V_VT(&var)=VT_BSTR;
 
    pList->ResetPropertyItem(var);
    VariantClear(&var);
}
 
void TestResetItem()
{
    IADsPropertyEntry *pEntry = NULL;
    IADsPropertyList *pList = NULL;
    long count;
    BSTR bstr;
    HRESULT hr;
 
    pList = GetPropertyCache(L"WinNT://myComputer,computer");
 
    hr = pList->get_PropertyCount(&count);
    if(SUCCEEDED(hr))
    {
        printf(" Count before item reset : %d\n",count);
    }
 
    printf("Walking up the property list before item reset: \n");
    for (int i=0; i<count; i++)
    {
        pEntry = GetNextEntry(pList);
        hr = pEntry->get_Name(&bstr);
        if(SUCCEEDED(hr))
        {
            printf("   Name : %S\n",bstr);
            SysFreeString(bstr);
        }
    }
 
    pList->Reset();   // Move the cursor to the beginning of the list.
 
    ResetItem(pList, L"Owner");
 
    hr = pList->get_PropertyCount(&count);
    if(SUCCEEDED(hr))
    {
        printf(" Count after item reset : %d\n",count);
    }
 
    printf("Walking up the property list after item reset: \n");
 
    for (i=0; i<count; i++)
    {
        pEntry = GetNextEntry(pList);
        hr = pEntry->get_Name(&bstr);
        if(SUCCEEDED(hr))
        {
            printf("   Name : %S\n",bstr);
            SysFreeString(bstr);
        }
    }
 
    pEntry->Release();
    pList->Release();
}
```





## -see-also




<a href="https://msdn.microsoft.com/573889e4-37af-4aca-afd7-ef06bcf8aa0d">ADSI Error Codes</a>



<a href="https://msdn.microsoft.com/70e9ce0e-ae83-43b7-8b84-99d5e1f8a8d2">IADsPropertyList</a>



<a href="https://msdn.microsoft.com/3564b61a-5950-4d00-8ea1-86fecd5c6c4e">IADsPropertyList Property Methods</a>



<a href="https://msdn.microsoft.com/6e103872-ea2e-4178-9c8a-b958ae3bcf85">IADsPropertyList::Item</a>



<a href="https://msdn.microsoft.com/2a12ba88-363b-41e3-bd05-8a71f5317097">IADsPropertyList::Next</a>
 

 

