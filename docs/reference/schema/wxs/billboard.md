---
custom_edit_url: null
sidebar_position: 12
---
# Billboard element
Billboard to display during install of a Feature

## Windows Installer references
[Billboard Table](https://docs.microsoft.com/en-us/windows/win32/msi/billboard-table), [BBControl Table](https://docs.microsoft.com/en-us/windows/win32/msi/bbcontrol-table)

## Parents
[BillboardAction](billboardaction.md)

## Children
* [Control](control.md) : Only controls of static type such as: Text, Bitmap, Icon, or custom control can be placed on a billboard.

## Attributes
**Feature** (String)
  : Feature whose state determines if the Billboard is shown.

**Id** (String, required)
  : Unique identifier for the Billboard.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)