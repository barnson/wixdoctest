---
custom_edit_url: null
sidebar_position: 168
---
# PatchFamilyRef element
This will cause the entire contents of the Fragment containing the referenced PatchFamily to be used in the process of creating a patch.

## Parents
[Patch](patch.md), [PatchFamilyGroup](patchfamilygroup.md)

## Attributes
**Id** (String, required)
  : The identifier of the PatchFamily to reference.

**ProductCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : Specifies the ProductCode of the product that this family applies to.


## See also
[PatchFamily](patchfamily.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)