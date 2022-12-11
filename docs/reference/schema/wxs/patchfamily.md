---
custom_edit_url: null
sidebar_position: 165
---
# PatchFamily element
Collection of items that should be kept from the differences between two products.

## Parents
[Fragment](fragment.md), [Patch](patch.md), [PatchFamilyGroup](patchfamilygroup.md)

## Children
* [All](all.md) 
* [BinaryRef](binaryref.md) 
* [ComponentRef](componentref.md) 
* [CustomActionRef](customactionref.md) 
* [DigitalCertificateRef](digitalcertificateref.md) 
* [DirectoryRef](directoryref.md) 
* [FeatureRef](featureref.md) 
* [IconRef](iconref.md) 
* [PropertyRef](propertyref.md) 
* [UIRef](uiref.md) 
* [WixUI (Ui extension)](../ui/wixui.md) 

## Attributes
**Id** (String, required)
  : Identifier which indicates a sequence family to which this patch belongs.

**ProductCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : Specifies the ProductCode of the product that this family applies to.

**Supersede** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this value to 'yes' to indicate that this patch will supersede all previous patches in this patch family. The default value is 'no'.

**Version** (String, required)
  : Used to populate the sequence column of the MsiPatchSequence table in the final MSP file. Specified in x.x.x.x format. See documentation for Sequence column of MsiPatchSequence table in MSI SDK.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)