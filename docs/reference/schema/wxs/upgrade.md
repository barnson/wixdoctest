---
custom_edit_url: null
sidebar_position: 281
---
# Upgrade element
Upgrade info for a particular UpgradeCode

## Windows Installer references
[Upgrade Table](https://docs.microsoft.com/en-us/windows/win32/msi/upgrade-table)

## Parents
[Package](package.md), [Fragment](fragment.md)

## Children
* [Property](property.md) : Nesting a Property element under an Upgrade element has been deprecated. Please nest Property elements in any of the other supported locations.
* [UpgradeVersion](upgradeversion.md) 

## Attributes
**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : This value specifies the upgrade code for the products that are to be detected by the FindRelatedProducts action.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)