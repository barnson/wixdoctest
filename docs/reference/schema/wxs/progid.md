---
custom_edit_url: null
sidebar_position: 181
---
# ProgId element
ProgId registration for parent Component. If ProgId has an associated Class, it must be a child of that element.

## Windows Installer references
[ProgId Table](https://docs.microsoft.com/en-us/windows/win32/msi/progid-table), [Class Table](https://docs.microsoft.com/en-us/windows/win32/msi/class-table), [Registry Table](https://docs.microsoft.com/en-us/windows/win32/msi/registry-table), [Icon Table](https://docs.microsoft.com/en-us/windows/win32/msi/icon-table)

## Parents
[ProgId](progid.md), [Class](class.md), [Component](component.md)

## Children
* [Extension](extension.md) : Extensions that refer to this ProgId
* [ProgId](progid.md) : The version-independent ProgId must be the first child element of actual ProgId. Nesting other ProgId elements within the Version-independent ProgId will create COM+ aliases, see http://support.microsoft.com/kb/305745 for more information.

## Attributes
**Advertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : 

**Description** (String)
  : 

**Icon** (String)
  : For an advertised ProgId, the Id of an Icon element. For a non-advertised ProgId, this is the Id of a file containing an icon resource.

**IconIndex** (Integer)
  : 

**Id** (String, required)
  : 

**NoOpen** (String)
  : Specifies that the associated ProgId should not be opened by users. The value is presented as a warning to users. An empty string is also valid for this attribute.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)