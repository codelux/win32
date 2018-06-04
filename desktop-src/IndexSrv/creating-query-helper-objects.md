---
Description: Creating Query Helper Objects
ms.assetid: 6a0b4a98-ba21-427d-8db3-3deed4874895
title: Creating Query Helper Objects
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Creating Query Helper Objects

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

The [Query Helper API](https://www.bing.com/search?q=Query Helper API) provides the [**Query**](iixssoquery.md) and [**Utility**](iixssoutil.md) objects for creating and managing queries to the [OLE DB Provider for Indexing Service](ole-db-provider-for-indexing-service.md). An application can use these objects along with an ADO [**Recordset**](https://www.bing.com/search?q=**Recordset**) object (see [Creating ADO Objects](creating-ado-objects.md)) that represents the resulting records from a query.

The following table shows how to declare a [**Query**](iixssoquery.md) object with either early or late binding.



| Object                                  | Early Binding                                                                                       | Late Binding                        |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------|-------------------------------------|
| [**Query**](iixssoquery.md)<br/> | `Dim objQuery as IXSSO.Query`<br/> Or<br/> `Reference to Cisso Type Library`<br/> | `Dim objQuery as Object`<br/> |



 

You subsequently can use either of the following statements to create the [**Query**](iixssoquery.md) object.


```VB
Set objQuery = New IXSSO.Query
Set objQuery = CreateObject("IXSSO.Query")
```



The following table shows how to declare a [**Utility**](iixssoutil.md) object with either early or late binding.



| Object                                   | Early Binding                                                                                        | Late Binding                          |
|------------------------------------------|------------------------------------------------------------------------------------------------------|---------------------------------------|
| [**Utility**](iixssoutil.md)<br/> | `Dim objUtility as IXSSO.Util`<br/> Or<br/> `Reference to Cisso Type Library`<br/> | `Dim objUtility as Object`<br/> |



 

You subsequently can use either of the following statements to create the [**Utility**](iixssoutil.md) object.


```VB
Set objUtility = New IXSSO.Util
Set objUtility = CreateObject("IXSSO.Util")
```



 

 



