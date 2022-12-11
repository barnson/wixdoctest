---
custom_edit_url: null
sidebar_position: 72
---
# DirectorySearchRef element
References an existing DirectorySearch element.

## Parents
[DirectorySearch](directorysearch.md), [DirectorySearchRef](directorysearchref.md), [ComponentSearch](componentsearch.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md), [ComplianceDrive](compliancedrive.md), [Property](property.md)

## Children
* [DirectorySearch](directorysearch.md) (no more than 1) 
* [DirectorySearchRef](directorysearchref.md) (no more than 1) 
* [FileSearch](filesearch.md) (no more than 1) 
* [FileSearchRef](filesearchref.md) (no more than 1) 

## Remarks
<p>A reference to another DirectorySearch element must reference the same Id, the same Parent Id, and the same Path. If any of these attribute values are different you must instead use a DirectorySearch element.</p>


## Attributes
**Id** (String, required)
  : Id of the search being referred to.

**Parent** (String)
  : This attribute is the signature of the parent directory of the file or directory in the Signature_ column. If this field is null, and the Path column does not expand to a full path, then all the fixed drives of the user's system are searched by using the Path. This field is a key into one of the following tables: the RegLocator, the IniLocator, the CompLocator, or the DrLocator tables.

**Path** (String)
  : Path on the user's system. Either absolute, or relative to containing directories.


## See also
[ComponentSearch](componentsearch.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)