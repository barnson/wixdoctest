---
custom_edit_url: null
sidebar_position: 88
---
# ExternalFile element
Contains information about specific files that are not part of a regular target image.

## Parents
[Family](family.md)

## Children
* [IgnoreRange](ignorerange.md) 
* [ProtectRange](protectrange.md) (required, ) 
* [SymbolPath](symbolpath.md) 

## Attributes
**File** (String, required)
  : Foreign key into the File table.

**Order** (xs:int, required)
  : Specifies the order of the external files to use when creating the patch.

**Source** (String)
  : Full path of the external file.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)