---
custom_edit_url: null
sidebar_position: 139
---
# MIME element
MIME content-type for an Extension

## Windows Installer references
[MIME Table](https://docs.microsoft.com/en-us/windows/win32/msi/mime-table)

## Parents
[Extension](extension.md)

## Attributes
**Advertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether this MIME is to be advertised. The default is to match whatever the parent extension element uses. If the parent element is not advertised, then this element cannot be advertised either.

**Class** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : Class ID for the COM server that is to be associated with the MIME content.

**ContentType** (String, required)
  : This is the identifier for the MIME content. It is commonly written in the form of type/format.

**Default** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If 'yes', become the content type for the parent Extension. The default value is 'no'.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)