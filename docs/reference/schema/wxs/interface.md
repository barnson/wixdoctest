---
custom_edit_url: null
sidebar_position: 123
---
# Interface element
COM Interface registration for parent TypeLib.

## Windows Installer references
[Registry Table](https://docs.microsoft.com/en-us/windows/win32/msi/registry-table)

## Parents
[TypeLib](typelib.md), [Class](class.md), [Component](component.md)

## Attributes
**BaseInterface** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : Identifies the interface from which the current interface is derived.

**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : GUID identifier for COM Interface.

**Name** (String, required)
  : Name for COM Interface.

**NumMethods** (Integer)
  : Number of methods implemented on COM Interface.

**ProxyStubClassId** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : GUID CLSID for proxy stub to COM Interface.

**ProxyStubClassId32** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : GUID CLSID for 32-bit proxy stub to COM Interface.

**Versioned** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Determines whether a Typelib version entry should be created with the other COM Interface registry keys. Default is 'yes'.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)