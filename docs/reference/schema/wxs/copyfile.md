---
custom_edit_url: null
sidebar_position: 49
---
# CopyFile element
Copy or move an existing file on the target machine, or copy a file that is being installed, to another destination. When this element is nested under a File element, the parent file will be installed, then copied to the specified destination if the parent component of the file is selected for installation or removal. When this element is nested under a Component element and no FileId attribute is specified, the file to copy or move must already be on the target machine. When this element is nested under a Component element and the FileId attribute is specified, the specified file is installed, then copied to the specified destination if the parent component is selected for installation or removal (use this option to control the copy of a file in a different component by the parent component's installation state). If the specified destination directory is the same as the directory containing the original file and the name for the proposed source file is the same as the original, then no action takes place.

## Windows Installer references
[DuplicateFile Table](https://docs.microsoft.com/en-us/windows/win32/msi/duplicatefile-table), [MoveFile Table](https://docs.microsoft.com/en-us/windows/win32/msi/movefile-table)

## Parents
[File](file.md), [Component](component.md)

## Attributes
**Delete** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute cannot be specified if the element is nested under a File element or the FileId attribute is specified. In other cases, if the attribute is not specified, the default value is "no" and the file is copied, not moved. Set the value to "yes" in order to move the file (thus deleting the source file) instead of copying it.

**DestinationDirectory** (String)
  : Set this value to the destination directory where an existing file on the target machine should be moved or copied to. This Directory must exist in the installer database at creation time. This attribute cannot be specified in conjunction with DestinationProperty.

**DestinationName** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : In prior versions of the WiX toolset, this attribute specified the short file name. Now set this value to the localizable name to be given to the original file after it is moved or copied. If this attribute is not specified, then the destination file is given the same name as the source file. If a short file name is specified, the DestinationShortName attribute may not be specified. Also, if this value is a long file name, the DestinationShortName attribute may be omitted to allow WiX to attempt to generate a unique short file name. However, if this name collides with another file or you wish to manually specify the short file name, then the DestinationShortName attribute may be specified.

**DestinationProperty** (String)
  : Set this value to a property that will have a value that resolves to the full path of the destination directory. The property does not have to exist in the installer database at creation time; it could be created at installation time by a custom action, on the command line, etc. This attribute cannot be specified in conjunction with DestinationDirectory.

**DestinationShortName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short file name of the file in 8.3 format. This attribute should only be set if there is a conflict between generated short file names or you wish to manually specify the short file name.

**FileId** (String)
  : This attribute cannot be specified if the element is nested under a File element. Set this attribute's value to the identifier of a file from a different component to copy it based on the install state of the parent component.

**Id** (String, required)
  : Primary key used to identify this particular entry.

**SourceDirectory** (String)
  : This attribute cannot be specified if the element is nested under a File element or the FileId attribute is specified. Set this value to the source directory from which to copy or move an existing file on the target machine. This Directory must exist in the installer database at creation time. This attribute cannot be specified in conjunction with SourceProperty.

**SourceName** ([WildCardLongFileNameType](wildcardlongfilenametype.md 'Values of this type will look like: "Long File N?me.extension*". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ | > : / " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : This attribute cannot be specified if the element is nested under a File element or the FileId attribute is specified. Set this value to the localizable name of the file(s) to be copied or moved. All of the files that match the wild card will be removed from the specified directory. The value is a filename that may also contain the wild card characters "?" for any single character or "*" for zero or more occurrences of any character. If this attribute is not specified (and this element is not nested under a File element or specify a FileId attribute) then the SourceProperty attribute should be set to the name of a property that will resolve to the full path of the source filename. If the value of this attribute contains a "*" wildcard and the DestinationName attribute is specified, all moved or copied files retain the file names from their sources.

**SourceProperty** (String)
  : This attribute cannot be specified if the element is nested under a File element or the FileId attribute is specified. Set this value to a property that will have a value that resolves to the full path of the source directory (or full path including file name if SourceName is not specified). The property does not have to exist in the installer database at creation time; it could be created at installation time by a custom action, on the command line, etc. This attribute cannot be specified in conjunction with SourceDirectory.


## See also
[RemoveFile](removefile.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)