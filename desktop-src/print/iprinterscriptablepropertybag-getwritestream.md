---
Description: Gets a stream and uses it to write to a stream property.
ms.assetid: EFF55B5C-55E2-4E03-9D96-FDB1BC550A53
title: IPrinterScriptablePropertyBag::GetWriteStream method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IPrinterScriptablePropertyBag::GetWriteStream method

Gets a stream and uses it to write to a stream property.

## Syntax


```C++
HRESULT GetWriteStream(
  [in]          BSTR                      bstrName,
  [out, retval] IPrinterScriptableStream **ppStream
);
```



## Parameters

<dl> <dt>

 *bstrName* \[in\]
</dt> <dd>

The property to write.

</dd> <dt>

*ppStream* \[out, retval\]
</dt> <dd>

The retrieved stream.

</dd> </dl>

## Return value

This method returns an **HRESULT** value.

## Remarks

**GetWriteStream** does not work with non-stream properties.

A call to **GetWriteStream** will throw an exception, if the specified property is not found. We recommend that you use a try-catch statement around calls to this method, to allow your app to handle any failures gracefully.

## Requirements



|                                     |                                                                                               |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8<br/>                                                                          |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                                |
| Target platform<br/>          | <dl> <dt>Desktop</dt> </dl>            |
| Header<br/>                   | <dl> <dt>Printerextension.h</dt> </dl> |



## See also

<dl> <dt>

[**IPrinterScriptablePropertyBag**](iprinterscriptablepropertybag.md)
</dt> <dt>

[**IPrinterScriptableStream**](iprinterscriptablestream.md)
</dt> </dl>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bprint\print%5D:%20IPrinterScriptablePropertyBag::GetWriteStream%20method%20%20RELEASE:%20%285/12/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")




