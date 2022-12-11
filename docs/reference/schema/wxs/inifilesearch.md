---
custom_edit_url: null
sidebar_position: 109
---
# IniFileSearch element
Searches for file, directory or registry key and assigns to value of parent Property

## Windows Installer references
[IniLocator Table](https://docs.microsoft.com/en-us/windows/win32/msi/inilocator-table), [Signature Table](https://docs.microsoft.com/en-us/windows/win32/msi/signature-table)

## Parents
[ComplianceCheck](compliancecheck.md), [Property](property.md)

## Children
* [DirectorySearch](directorysearch.md) (no more than 1) 
* [DirectorySearchRef](directorysearchref.md) (no more than 1) 
* [FileSearch](filesearch.md) (no more than 1) 
* [FileSearchRef](filesearchref.md) (no more than 1) 

## Attributes
**Field** (Integer)
  : The field in the .ini line. If field is Null or 0, the entire line is read.

**Id** (String, required)
  : External key into the Signature table.

**Key** (String, required)
  : The key value within the section.

**Name** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'), required)
  : In prior versions of the WiX toolset, this attribute specified the short name. This attribute's value may now be either a short or long name. If a short name is specified, the ShortName attribute may not be specified. Also, if this value is a long name, the ShortName attribute may be omitted to allow WiX to attempt to generate a unique short name. However, if you wish to manually specify the short name, then the ShortName attribute may be specified.

**Section** (String, required)
  : The localizable .ini file section.

**ShortName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short name of the file in 8.3 format. This attribute should only be set if the user wants to manually specify the short name.

**Type** (enumeration)
  : Must be file if last child is FileSearch element and must be directory if last child is DirectorySearch element. This attribute's value must be one of the following:
- *directory*: A directory location.
- *file*: A file location. This is the default value.
- *raw*: A raw .ini value.


## See also
[ComponentSearch](componentsearch.md), [RegistrySearch](registrysearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)