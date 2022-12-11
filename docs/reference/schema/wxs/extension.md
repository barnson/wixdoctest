---
custom_edit_url: null
sidebar_position: 87
---
# Extension element
Extension for a Component

## Windows Installer references
[MIME Table](https://docs.microsoft.com/en-us/windows/win32/msi/mime-table), [Verb Table](https://docs.microsoft.com/en-us/windows/win32/msi/verb-table), [Registry Table](https://docs.microsoft.com/en-us/windows/win32/msi/registry-table)

## Parents
[ProgId](progid.md), [Component](component.md)

## Children
* [MIME](mime.md) 
* [Verb](verb.md) 

## Attributes
**Advertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether this extension is to be advertised. The default is "no".

**ContentType** (String)
  : The MIME type that is to be written.

**Id** (String, required)
  : This is simply the file extension, like "doc" or "xml". Do not include the preceding period.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)