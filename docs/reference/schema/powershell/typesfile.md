---
custom_edit_url: null
sidebar_position: 3
---
# TypesFile element (Powershell extension)
Identifies the parent File as a types XML file for the referenced PowerShell snap-in.

## Parents
[File](../wxs/file.md), [SnapIn](snapin.md)

## Remarks
A types XML file used by the extensible type system.


## Attributes
**FileId** (String)
  : Reference to the types File ID. This is required when nested under the SnapIn element.

**SnapIn** (String)
  : Reference to the PowerShell snap-in ID for which this types file is associated. This is required when nested under the File element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/ps.xsd)