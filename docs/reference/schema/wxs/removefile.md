---
custom_edit_url: null
sidebar_position: 214
---
# RemoveFile element
Remove a file(s) if the parent component is selected for installation or removal. Multiple files can be removed by specifying a wildcard for the value of the Name attribute. By default, the source directory of the file is the directory of the parent component. This can be overridden by specifying the Directory attribute with a value corresponding to the Id of the source directory, or by specifying the Property attribute with a value corresponding to a property that will have a value that resolves to the full path to the source directory.

## Windows Installer references
[RemoveFile Table](https://docs.microsoft.com/en-us/windows/win32/msi/removefile-table)

## Parents
[Component](component.md)

## Attributes
**Directory** (String)
  : Overrides the directory of the parent component with a specific Directory. This Directory must exist in the installer database at creation time. This attribute cannot be specified in conjunction with the Property attribute.

**Id** (String)
  : Primary key used to identify this particular entry.

**Name** ([WildCardLongFileNameType](wildcardlongfilenametype.md 'Values of this type will look like: "Long File N?me.extension*". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ | > : / " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'), required)
  : This value should be set to the localizable name of the file(s) to be removed. All of the files that match the wild card will be removed from the specified directory. The value is a filename that may also contain the wild card characters "?" for any single character or "*" for zero or more occurrences of any character. In prior versions of the WiX toolset, this attribute specified the short file name. This attribute's value may now be either a short or long file name. If a short file name is specified, the ShortName attribute may not be specified. Also, if this value is a long file name, the ShortName attribute may be omitted to allow WiX to attempt to generate a unique short file name. However, if you wish to manually specify the short file name, then the ShortName attribute may be specified.

**On** (enumeration, required)
  : This value determines the time at which the file(s) may be removed. For 'install', the file will be removed only when the parent component is being installed (msiInstallStateLocal or msiInstallStateSource); for 'uninstall', the file will be removed only when the parent component is being removed (msiInstallStateAbsent); for 'both', the file will be removed in both cases. This attribute's value must be one of the following:
- *install*: The action should happen during install (msiInstallStateLocal or msiInstallStateSource).
- *uninstall*: The action should happen during uninstall (msiInstallStateAbsent).
- *both*: The action should happen during both install and uninstall.

**Property** (String)
  : Overrides the directory of the parent component with the value of the specified property. The property should have a value that resolves to the full path of the source directory. The property does not have to exist in the installer database at creation time; it could be created at installation time by a custom action, on the command line, etc. This attribute cannot be specified in conjunction with the Directory attribute.

**ShortName** ([WildCardShortFileNameType](wildcardshortfilenametype.md 'Values of this type will look like: "File?.*". Only one period is allowed. The following characters are not allowed: \ | > : / " + , ; = [ ] <, or whitespace. The name cannot be longer than 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short file name of the file in 8.3 format. This attribute should only be set if you want to manually specify the short file name.

**Subdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the Directory attribute or parent Directory reference for the file to be removed.


## See also
[CopyFile](copyfile.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)