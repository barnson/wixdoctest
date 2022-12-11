---
custom_edit_url: null
sidebar_position: 4
---
# All element
Used only for PatchFamilies to include all changes between the baseline and upgraded packages in a patch.

## Parents
[PatchFamily](patchfamily.md)

## Remarks
<p>Warning: this is intended for testing purposes only. Shipping a patch with all changes negates the benefits of using patch families for including only specific changes.</p>
<p>Because changing the ProductCode is not supported in a patch, the ProductCode property is automatically removed from the transform.</p>


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)