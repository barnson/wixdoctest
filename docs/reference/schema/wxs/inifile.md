---
custom_edit_url: null
sidebar_position: 108
---
# IniFile element
Adds or removes .ini file entries.

## Windows Installer references
[IniFile Table](https://docs.microsoft.com/en-us/windows/win32/msi/inifile-table), [RemoveIniFile Table](https://docs.microsoft.com/en-us/windows/win32/msi/removeinifile-table)

## Parents
[Component](component.md)

## Attributes
**Action** (enumeration, required)
  : The type of modification to be made. This attribute's value must be one of the following:
- *addLine*: Creates or updates an .ini entry.
- *addTag*: Creates a new entry or appends a new comma-separated value to an existing entry.
- *createLine*: Creates an .ini entry only if the entry does no already exist.
- *removeLine*: Removes an .ini entry.
- *removeTag*: Removes a tag from an .ini entry.

**Directory** (String)
  : Name of a property, the value of which is the full path of the folder containing the .ini file. Can be name of a directory in the Directory table, a property set by the AppSearch table, or any other property representing a full path.

**Id** (String, required)
  : Identifier for ini file.

**Key** (String, required)
  : The localizable .ini file key within the section.

**Name** ([LongFileNameType](longfilenametype.md 'Values of this type will look like: "Long File Name.extension". Legal long names contain no more than 260 characters and must contain at least one non-period character. The following characters are not allowed: \ ? | > : / * " or <. The name must be shorter than 260 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'), required)
  : In prior versions of the WiX toolset, this attribute specified the short name. This attribute's value may now be either a short or long name. If a short name is specified, the ShortName attribute may not be specified. Also, if this value is a long name, the ShortName attribute may be omitted to allow WiX to attempt to generate a unique short name. However, if this name collides with another file or you wish to manually specify the short name, then the ShortName attribute may be specified.

**Section** (String, required)
  : The localizable .ini file section.

**ShortName** ([ShortFileNameType](shortfilenametype.md 'Values of this type will look like: "FileName.ext". Only one period is allowed. The following characters are not allowed: \ ? | > : / * " + , ; = [ ] <, or whitespace. The name cannot exceed 8 characters and the extension cannot exceed 3 characters. The value could also be a localization variable with the format !(loc.VARIABLE).'))
  : The short name of the in 8.3 format. This attribute should only be set if there is a conflict between generated short names or the user wants to manually specify the short name.

**Value** (String)
  : The localizable value to be written or deleted. This attribute must be set if the Action attribute's value is "addLine", "addTag", or "createLine".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)