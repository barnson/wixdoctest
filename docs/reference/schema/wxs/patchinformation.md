---
custom_edit_url: null
sidebar_position: 170
---
# PatchInformation element
Properties about the patch to be placed in the Summary Information Stream. These are visible from COM through the IStream interface, and these properties can be seen on the package in Explorer.

## Parents
[Patch](patch.md), [PatchCreation](patchcreation.md)

## Remarks
<p>You can specify any valid Windows code by by integer like 1252, or by web name like Windows-1252. See [Code pages](reference/codepage.md) for more information.</p>


## Attributes
**AdminImage** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Deprecated

**Comments** (String)
  : General purpose of the patch package. For example, "This patch contains the logic and data required to install _product_."

**Compressed** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Deprecated

**Description** (String)
  : A short description of the patch that includes the name of the product.

**Keywords** (String)
  : A semicolon-delimited list of network or URL locations for alternate sources of the patch. The default is "Installer,Patching,PCP,Database".

**Languages** (String)
  : Deprecated

**Manufacturer** (String)
  : The name of the manufacturer of the patch package.

**Platforms** (String)
  : Deprecated

**ReadOnly** ([YesNoDefaultTypeUnion](yesnodefaulttype.md 'Values of this type will either be "default", "yes", or "no".'))
  : The value of this attribute conveys whether the package should be opened as read-only. A database editing tool should not modify a read-only enforced database and should issue a warning at attempts to modify a read-only recommended database.

**ShortNames** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Deprecated

**SummaryCodepage** (String)
  : The code page integer value or web name for summary info strings only. The default is 1252. See remarks for more information.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)