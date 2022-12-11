---
custom_edit_url: null
sidebar_position: 172
---
# PatchProperty element
A property for this patch database.

## Windows Installer references
[MsiPatchMetadata Table](https://docs.microsoft.com/en-us/windows/win32/msi/msipatchmetadata-table)

## Parents
[Patch](patch.md), [PatchCreation](patchcreation.md)

## Remarks
<p>When authored under the Patch element, the PatchProperty defines entries in the MsiPatchMetadata table.</p>


## Attributes
**Company** (String)
  : Name of the company for a custom metadata property.

**Name** (String, required)
  : Name of the patch property.

**Value** (String, required)
  : Value of the patch property.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)