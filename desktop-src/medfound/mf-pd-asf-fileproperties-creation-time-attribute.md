﻿---
Description: 'Specifies the date and time when an Advanced Systems Format (ASF) file was created.'
ms.assetid: '97f80584-9d74-4ba5-80f4-ddb6f2bc4625'
title: 'MF\_PD\_ASF\_FILEPROPERTIES\_CREATION\_TIME attribute'
---

# MF\_PD\_ASF\_FILEPROPERTIES\_CREATION\_TIME attribute

Specifies the date and time when an Advanced Systems Format (ASF) file was created.

## Data type

Byte array

## Remarks

This attribute applies to presentation descriptors for ASF content. The value of the attribute is a **FILETIME** structure, which is documented in the Windows SDK.

The [**IMFASFContentInfo::GeneratePresentationDescriptor**](imfasfcontentinfo-generatepresentationdescriptor.md) method generates this attribute from the ASF metadata.

## Requirements



|                                     |                                                                                          |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                           |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                     |
| Header<br/>                   | <dl> <dt>Wmcontainer.h</dt> </dl> |



## See also

<dl> <dt>

[Alphabetical List of Media Foundation Attributes](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**IMFAttributes::GetBlob**](imfattributes-getblob.md)
</dt> <dt>

[**IMFAttributes::SetBlob**](imfattributes-setblob.md)
</dt> <dt>

[**IMFPresentationDescriptor**](imfpresentationdescriptor.md)
</dt> <dt>

[Presentation Descriptor Attributes](presentation-descriptor-attributes.md)
</dt> <dt>

[ASF Header Object](asf-file-structure.md#header-object)
</dt> <dt>

[Presentation Descriptors](presentation-descriptors.md)
</dt> </dl>

 

 



