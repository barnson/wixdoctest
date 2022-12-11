---
custom_edit_url: null
sidebar_position: 97
---
# FileSearch element
Searches for file and assigns to fullpath value of parent Property

## Windows Installer references
[DrLocator Table](https://docs.microsoft.com/en-us/windows/win32/msi/drlocator-table), [Signature Table](https://docs.microsoft.com/en-us/windows/win32/msi/signature-table)

## Parents
[DirectorySearch](directorysearch.md), [DirectorySearchRef](directorysearchref.md), [ComponentSearch](componentsearch.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md)

## Remarks
<a>When the parent DirectorySearch/@Depth attribute is greater than 0, the FileSearch/@Id attribute must be absent or the same as the parent DirectorySearch/@Id attribute value, unless the parent DirectorySearch/@AssignToProperty attribute value is 'yes'.</a>


## Attributes
**Id** (String)
  : Unique identifier for the file search and external key into the Signature table. If this attribute value is not set then the parent element's @Id attribute is used.

**Languages** (String)
  : The languages supported by the file.

**MaxDate** (xs:dateTime)
  : The maximum modification date and time of the file. Formatted as YYYY-MM-DDTHH:mm:ss, where YYYY is the year, MM is month, DD is day, 'T' is literal, HH is hour, mm is minute and ss is second.

**MaxSize** (xs:int)
  : The maximum size of the file.

**MaxVersion** (String)
  : The maximum version of the file.

**MinDate** (xs:dateTime)
  : The minimum modification date and time of the file. Formatted as YYYY-MM-DDTHH:mm:ss, where YYYY is the year, MM is month, DD is day, 'T' is literal, HH is hour, mm is minute and ss is second.

**MinSize** (xs:int)
  : The minimum size of the file.

**MinVersion** (String)
  : The minimum version of the file.

**Name** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : In prior versions of the WiX toolset, this attribute specified the short file name. This attribute's value may now be either a short or long file name. If a short file name is specified, the ShortName attribute may not be specified. If you wish to manually specify the short file name, then the ShortName attribute may be specified.

**ShortName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short file name of the file in 8.3 format. There is a Windows Installer bug which prevents the FileSearch functionality from working if both a short and long file name are specified. Since the Name attribute allows either a short or long name to be specified, it is the only attribute related to file names which should be specified.


## See also
[ComponentSearch](componentsearch.md), [DirectorySearch](directorysearch.md), [DirectorySearchRef](directorysearchref.md), [FileSearchRef](filesearchref.md), [IniFileSearch](inifilesearch.md), [RegistrySearch](registrysearch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)