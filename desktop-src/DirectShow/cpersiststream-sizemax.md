---
Description: 'Retrieves the maximum byte size needed for the current stream, not including the version number.'
ms.assetid: 'ca1a68e2-02b4-4eea-916a-e0418ae811ae'
title: 'CPersistStream.SizeMax method'
---

# CPersistStream.SizeMax method

Retrieves the maximum byte size needed for the current stream, not including the version number.

## Syntax


```C++
virtual int SizeMax();
```



## Parameters

This method has no parameters.

## Return value

Returns the number of bytes needed for data, not including the version number.

## Remarks

The default version returns zero; it should be overridden to provide some other appropriate value.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Pstream.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CPersistStream Class**](cpersiststream.md)
</dt> </dl>

�

�



