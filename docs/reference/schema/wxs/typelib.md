---
custom_edit_url: null
sidebar_position: 267
---
# TypeLib element
Register a type library (TypeLib). Please note that in order to properly use this non-advertised, you will need use this element with Advertise='no' and also author the appropriate child Interface elements by extracting them from the type library itself.

## Windows Installer references
[TypeLib Table](https://docs.microsoft.com/en-us/windows/win32/msi/typelib-table), [Registry Table](https://docs.microsoft.com/en-us/windows/win32/msi/registry-table)

## Parents
[File](file.md), [Component](component.md)

## Children
* [AppId](appid.md) 
* [Class](class.md) 
* [Interface](interface.md) 

## Attributes
**Advertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Value of 'yes' will create a row in the TypeLib table. Value of 'no' will create rows in the Registry table. The default value is 'no'.

**Control** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Value of 'yes' means the type library describes controls, and should not be displayed in type browsers intended for nonvisual objects. This attribute can only be set if Advertise='no'.

**Cost** (xs:int)
  : The cost associated with the registration of the type library in bytes. This attribute cannot be set if Advertise='no'.

**Description** (String)
  : The localizable description of the type library.

**HasDiskImage** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Value of 'yes' means the type library exists in a persisted form on disk. This attribute can only be set if Advertise='no'.

**HelpDirectory** (String)
  : The identifier of the Directory element for the help directory.

**HelpSubirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the HelpDirectory attribute for the typelib's help directory.

**Hidden** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Value of 'yes' means the type library should not be displayed to users, although its use is not restricted. Should be used by controls. Hosts should create a new type library that wraps the control with extended properties. This attribute can only be set if Advertise='no'.

**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : The GUID that identifes the type library.

**Language** (Integer, required)
  : The language of the type library. This must be a non-negative integer.

**MajorVersion** (Integer)
  : The major version of the type library. The value should be an integer from 0 - 255.

**MinorVersion** (Integer)
  : The minor version of the type library. The value should be an integer from 0 - 255.

**ResourceId** (Integer)
  : The resource id of a typelib. The value is appended to the end of the typelib path in the registry.

**Restricted** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Value of 'yes' means the type library is restricted, and should not be displayed to users. This attribute can only be set if Advertise='no'.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)