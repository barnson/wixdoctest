---
custom_edit_url: null
sidebar_position: 52
---
# CreateFolder element
Create folder as part of parent Component.

## Windows Installer references
[CreateFolder Table](https://docs.microsoft.com/en-us/windows/win32/msi/createfolder-table)

## Parents
[Component](component.md)

## Children
* [Permission](permission.md) : ACL permission
* [PermissionEx (Util extension)](../util/permissionex.md) 
* [Shortcut](shortcut.md) : Non-advertised shortcut to this folder, Shortcut Target is preset to the folder

## Attributes
**Directory** (String)
  : Identifier of Directory to create. Defaults to Directory of parent Component.

**Subdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the Directory attribute or parent Directory reference for the directory to be created.


## See also
[RemoveFolder](removefolder.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)