---
custom_edit_url: null
sidebar_position: 14
---
# Binary element
Binary data used for CustomAction elements and UI controls.

## Windows Installer references
[Binary Table](https://docs.microsoft.com/en-us/windows/win32/msi/binary-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [Control](control.md), [UI](ui.md)

## Attributes
**Id** (String, required)
  : The Id cannot be longer than 55 characters.  In order to prevent errors in cases where the Id is modularized, it should not be longer than 18 characters.

**SourceFile** (String)
  : Path to the binary file.

**SuppressModularization** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Use to suppress modularization of this Binary identifier in merge modules.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)