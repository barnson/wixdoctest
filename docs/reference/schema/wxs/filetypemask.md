---
custom_edit_url: null
sidebar_position: 99
---
# FileTypeMask element
FileType data for class Id registration.

## Parents
[Class](class.md)

## Attributes
**Mask** ([HexType](hextype.md 'This type supports any hexadecimal number. Both upper and lower case are supported for letters appearing in the number. This type also includes the empty string: "".'), required)
  : Hex value that is AND'd against the bytes in the file at Offset.

**Offset** (Integer, required)
  : Offset into file. If positive, offset is from the beginning; if negative, offset is from the end.

**Value** ([HexType](hextype.md 'This type supports any hexadecimal number. Both upper and lower case are supported for letters appearing in the number. This type also includes the empty string: "".'), required)
  : If the result of the AND'ing of Mask with the bytes in the file is Value, the file is a match for this File Type.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)