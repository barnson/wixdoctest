---
custom_edit_url: null
sidebar_position: 283
---
# UpgradeImage element
Contains information about the upgraded images of the product.

## Parents
[Family](family.md)

## Children
* [SymbolPath](symbolpath.md) 
* [TargetImage](targetimage.md) 
* [UpgradeFile](upgradefile.md) 

## Attributes
**Id** (String, required)
  : Identifier to connect target images with upgraded image.

**SourceFile** (String)
  : Full path to location of msi file for upgraded image.

**SourcePatch** (String)
  : Modified copy of the upgraded installation database that contains additional authoring specific to patching.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)