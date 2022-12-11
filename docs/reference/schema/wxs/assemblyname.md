---
custom_edit_url: null
sidebar_position: 11
---
# AssemblyName element
The MsiAssemblyName table specifies the schema for the elements of a strong assembly cache name for a .NET Framework or Win32 assembly. Consider using the Assembly attribute on File element to have the toolset populate these entries automatically.

## Windows Installer references
[MsiAssemblyName Table](https://docs.microsoft.com/en-us/windows/win32/msi/msiassemblyname-table)

## Parents
[File](file.md)

## Attributes
**Id** (String, required)
  : Name of the attribute associated with the value specified in the Value column.

**Value** (String)
  : Value associated with the name specified in the Name column.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)