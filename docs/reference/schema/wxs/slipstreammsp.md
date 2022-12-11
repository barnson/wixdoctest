---
custom_edit_url: null
sidebar_position: 252
---
# SlipstreamMsp element
Specifies a patch included in the same bundle that is installed when the parent MSI package is installed.

## Parents
[MsiPackage](msipackage.md)

## Remarks
<p>You can also specify that any MspPackage elements in the chain are automatically slipstreamed by setting the Slipstream attribute of an MspPackage to "yes". This will reduce the amount of authoring you need to write and will determine which msi packages can slipstream patches when building a bundle.</p>


## Attributes
**Id** (String, required)
  : The identifier for a MspPackage in the bundle.


## See also
[MspPackage](msppackage.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)