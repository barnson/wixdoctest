---
custom_edit_url: null
sidebar_position: 263
---
# TargetProductCode element
A product code for a product that can accept the patch.

## Parents
[PatchCreation](patchcreation.md), [TargetProductCodes](targetproductcodes.md)

## Remarks
<p>When using the PatchCreation element, if the Id attribute value is '*' or this element is not authored, the product codes of all products referenced by the TargetImages element are used.</p>
<p>When using the Patch element, the Id attribute value must not be '*'. Use the TargetProductCodes/@Replace attribute instead.</p>


## Attributes
**Id** (String, required)
  : The product code for a product that can accept the patch. This can be '*'. See remarks for more information.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)