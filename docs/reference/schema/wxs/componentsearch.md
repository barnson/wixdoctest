---
custom_edit_url: null
sidebar_position: 43
---
# ComponentSearch element
Searches for file or directory and assigns to value of parent Property.

## Windows Installer references
[CompLocator Table](https://docs.microsoft.com/en-us/windows/win32/msi/complocator-table), [Signature Table](https://docs.microsoft.com/en-us/windows/win32/msi/signature-table)

## Parents
[ComplianceCheck](compliancecheck.md), [Property](property.md)

## Children
* [DirectorySearch](directorysearch.md) (no more than 1) 
* [DirectorySearchRef](directorysearchref.md) (no more than 1) 
* [FileSearch](filesearch.md) (no more than 1) 
* [FileSearchRef](filesearchref.md) (no more than 1) 

## Attributes
**Guid** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : The component ID of the component whose key path is to be used for the search.

**Id** (String, required)
  : 

**Type** (enumeration)
  : Must be file if last child is FileSearch element and must be directory if last child is DirectorySearch element. This attribute's value must be one of the following:
- *directory*: The key path of the component is a directory.
- *file*: The key path of the component is a file. This is the default value.


## See also
[IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)