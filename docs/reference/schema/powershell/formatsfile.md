---
custom_edit_url: null
sidebar_position: 1
---
# FormatsFile element (Powershell extension)
Identifies the parent File as a formats XML file for the referenced PowerShell snap-in.

## Parents
[File](../wxs/file.md), [SnapIn](snapin.md)

## Remarks
A formats XML file that defines output formats for objects on the pipeline.


## Attributes
**FileId** (String)
  : Reference to the formats File ID. This is required when nested under the SnapIn element.

**SnapIn** (String)
  : Reference to the PowerShell snap-in ID for which this formats file is associated. This is required when nested under the File element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/ps.xsd)