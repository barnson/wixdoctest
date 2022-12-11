---
custom_edit_url: null
sidebar_position: 250
---
# ShortcutProperty element
Property values for a shortcut. This element's functionality is available starting with MSI 5.0.

## Windows Installer references
[MsiShortcutProperty Table](https://docs.microsoft.com/en-us/windows/win32/msi/msishortcutproperty-table)

## Parents
[Shortcut](shortcut.md)

## Attributes
**Id** (String)
  : Unique identifier for MsiShortcutProperty table. If omitted, a stable identifier will be generated from the parent shortcut identifier and Key value.

**Key** (String, required)
  : A formatted string identifying the property to be set.

**Value** (String)
  : A formatted string supplying the value of the property.


## See also
[Shortcut](shortcut.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)