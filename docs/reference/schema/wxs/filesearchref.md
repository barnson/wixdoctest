---
custom_edit_url: null
sidebar_position: 98
---
# FileSearchRef element
References an existing FileSearch element.

## Parents
[DirectorySearch](directorysearch.md), [DirectorySearchRef](directorysearchref.md), [ComponentSearch](componentsearch.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md)

## Remarks
<p>A reference to another FileSearch element must reference the same Id and the same Parent Id. If any of these attribute values are different you must instead use a FileSearch element.</p>


## Attributes
**Id** (String, required)
  : Specify the Id to the FileSearch to reference.


## See also
[FileSearch](filesearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)