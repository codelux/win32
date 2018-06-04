---
Description: Create a Query Object
ms.assetid: e4d08430-5536-48da-8308-7af43e0154dc
title: Create a Query Object
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Create a Query Object

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

This code segment uses the **CreateObject** method of the **WScript** (Windows Script Host) object to create objQ, a [**Query**](iixssoquery.md) object, from Ixsso.dll


```VB
Set objQ = WScript.CreateObject("IXSSO.Query")
```



 

 


