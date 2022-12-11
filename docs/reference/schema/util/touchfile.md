---
custom_edit_url: null
sidebar_position: 37
---
# TouchFile element (Util extension)
Updates the last modified date/time of a file.

## Parents
[Component](../wxs/component.md)

## Attributes
**Id** (String)
  : Identifier for the touch file operation. If the identifier is not specified it will be generated.

**Nonvital** (wxs:YesNoTypeUnion)
  : Indicates the installation will succeed even if the modified time of the file cannot be updated. The default is 'no'.

**OnInstall** (wxs:YesNoTypeUnion)
  : Specifies whether or not the modified time of the file should be updated on install. If the OnInstall, OnReinstall and OnUninstall attributes are all absent the default is 'yes'.

**OnReinstall** (wxs:YesNoTypeUnion)
  : Specifies whether or not the modified time of the file should be updated on reinstall. If the OnInstall, OnReinstall and OnUninstall attributes are all absent the default is 'yes'.

**OnUninstall** (wxs:YesNoTypeUnion)
  : Specifies whether or not the modified time of the file should be updated on uninstall. If the OnInstall, OnReinstall and OnUninstall attributes are all absent the default is 'no'.

**Path** (String, required)
  : Path of the file to update. This value is formatted.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)