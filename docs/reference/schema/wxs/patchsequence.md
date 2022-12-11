---
custom_edit_url: null
sidebar_position: 173
---
# PatchSequence element
Sequence information for this patch database. Sequence information is generated automatically in most cases, and rarely needs to be set explicitly.

## Windows Installer references
[MsiPatchSequence Table](https://docs.microsoft.com/en-us/windows/win32/msi/msipatchsequence-table)

## Parents
[PatchCreation](patchcreation.md)

## Attributes
**PatchFamily** (String, required)
  : Identifier which indicates a sequence family to which this patch belongs.

**ProductCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : Specifies the ProductCode of the product that this family applies to. This attribute cannot the specified if the TargetImage attribute is specified.

**Sequence** (String)
  : Used to populate the sequence column of the MsiPatchSequence table in the final MSP file. Specified in x.x.x.x format. See documentation for Sequence column of MsiPatchSequence table in MSI SDK.

**Supersede** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this value to 'yes' to indicate that this patch will supersede all previous patches in this patch family. The default value is 'no'.

**Target** (String)
  : Deprecated: Use the TargetImage attribute instead.

**TargetImage** (String)
  : Specifies the TargetImage that this family applies to. This attribute cannot the specified if the ProductCode attribute is specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)