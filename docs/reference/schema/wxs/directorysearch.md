---
custom_edit_url: null
sidebar_position: 71
---
# DirectorySearch element
Searches for directory and assigns to value of parent Property.

## Windows Installer references
[DrLocator Table](https://docs.microsoft.com/en-us/windows/win32/msi/drlocator-table), [Signature Table](https://docs.microsoft.com/en-us/windows/win32/msi/signature-table)

## Parents
[DirectorySearch](directorysearch.md), [DirectorySearchRef](directorysearchref.md), [ComponentSearch](componentsearch.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md), [ComplianceDrive](compliancedrive.md), [ComplianceCheck](compliancecheck.md), [Property](property.md)

## Children
* [DirectorySearch](directorysearch.md) (no more than 1) 
* [DirectorySearchRef](directorysearchref.md) 
* [FileSearch](filesearch.md) (no more than 1) 
* [FileSearchRef](filesearchref.md) (no more than 1) 

## Remarks
<p>Use the AssignToProperty attribute to search for a file but set the outer property to the directory containing the file. When this attribute is set to 'yes', you may only nest a FileSearch element with a unique Id or define no child element.</p>
<a>When the parent DirectorySearch/@Depth attribute is greater than 0, the FileSearch/@Id attribute must be absent or the same as the parent DirectorySearch/@Id attribute value, unless the parent DirectorySearch/@AssignToProperty attribute value is 'yes'.</a>


## Attributes
**AssignToProperty** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set the value of the outer Property to the result of this search. See remarks for more information.

**Depth** (Integer)
  : Depth below the path that the installer searches for the file or directory specified by the search. See remarks for more information.

**Id** (String, required)
  : Unique identifier for the directory search.

**Path** (String)
  : Path on the user's system. Either absolute, or relative to containing directories.


## See also
[ComponentSearch](componentsearch.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)