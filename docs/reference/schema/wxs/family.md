---
custom_edit_url: null
sidebar_position: 90
---
# Family element
Group of one or more upgraded images of a product.

## Parents
[PatchCreation](patchcreation.md)

## Children
* [ExternalFile](externalfile.md) 
* [ProtectFile](protectfile.md) 
* [UpgradeImage](upgradeimage.md) 

## Attributes
**DiskId** ([DiskIdType](diskidtype.md 'Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.'))
  : Entered into the DiskId field of the new Media table record.

**DiskPrompt** (String)
  : Value to display in the "[1]" of the DiskPrompt Property. Using this attribute will require you to define a DiskPrompt Property.

**MediaSrcProp** (String)
  : Entered into the Source field of the new Media table entry of the upgraded image.

**Name** (String, required)
  : Identifier for the family.

**SequenceStart** (xs:int)
  : Sequence number for the starting file.

**VolumeLabel** (String)
  : Entered into the VolumeLabel field of the new Media table record.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)