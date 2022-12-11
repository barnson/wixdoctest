---
custom_edit_url: null
sidebar_position: 210
---
# RemoteRelatedBundle element
Defines a related bundle for the parent RemoteBundle.

## Parents
[RemoteBundle](remotebundle.md)

## Attributes
**Action** (enumeration, required)
  : The action to take on bundles related to this one. This attribute's value must be one of the following:
- *detect*
- *upgrade*
- *addon*
- *patch*

**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : The identifier of the RelatedBundle group.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)