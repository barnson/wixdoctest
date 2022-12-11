---
custom_edit_url: null
sidebar_position: 17
---
# FormatFile element (Util extension)
Formats a file's contents at install time. The contents are formatted according to the rules of the [Formatted](https://learn.microsoft.com/en-us/windows/win32/msi/formatted) data type.

## Parents
[File](../wxs/file.md)

## Attributes
**BinaryRef** (String, required)
  : The id of a Binary row that contains a copy of the file. The file in the Binary table overwrites whatever file is installed by the parent component.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)