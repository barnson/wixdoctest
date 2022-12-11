---
custom_edit_url: null
sidebar_position: 262
---
# TargetImage element
Contains information about the target images of the product.

## Parents
[UpgradeImage](upgradeimage.md)

## Children
* [SymbolPath](symbolpath.md) 
* [TargetFile](targetfile.md) 

## Attributes
**Id** (String, required)
  : Identifier for the target image.

**IgnoreMissingFiles** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Files missing from the target image are ignored by the installer.

**Order** (xs:int, required)
  : Relative order of the target image.

**SourceFile** (String)
  : Full path to the location of the msi file for the target image.

**Validation** (String)
  : Product checking to avoid applying irrelevant transforms.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)