---
custom_edit_url: null
sidebar_position: 155
---
# OptimizeCustomActions element
Indicates whether custom actions can be skipped when applying the patch.

## Windows Installer references
[MsiPatchMetadata Table](https://docs.microsoft.com/en-us/windows/win32/msi/msipatchmetadata-table)

## Parents
[Patch](patch.md), [PatchMetadata](patchmetadata.md)

## Attributes
**SkipAssignment** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Skip property (type 51) and directory (type 35) assignment custom actions.

**SkipDeferred** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Skip custom actions that run within the script.

**SkipImmediate** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Skip immediate custom actions that are not property or directory assignment custom actions.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)