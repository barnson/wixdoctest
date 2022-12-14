---
custom_edit_url: null
sidebar_position: 121
---
# Instance element
Defines an instance transform for your product.

## Parents
[InstanceTransforms](instancetransforms.md)

## Attributes
**Id** (String, required)
  : The identity of the instance transform. This value will define the name by which the instance should be referred to on the command line. In addition, the value of the this attribute will determine what the value of the property specified in Property attribute on InstanceTransforms will change to for each instance.

**ProductCode** ([AutogenGuid](autogenguid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". A GUID can be auto-generated by setting the value to "*". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : The ProductCode for this instance.

**ProductName** (String)
  : The ProductName for this instance.

**UpgradeCode** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : The UpgradeCode for this instance.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)