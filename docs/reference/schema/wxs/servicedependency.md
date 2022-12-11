---
custom_edit_url: null
sidebar_position: 240
---
# ServiceDependency element
Service or group of services that must start before the parent service.

## Windows Installer references
[ServiceInstall Table](https://docs.microsoft.com/en-us/windows/win32/msi/serviceinstall-table)

## Parents
[ServiceInstall](serviceinstall.md)

## Attributes
**Group** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to 'yes' to indicate that the value in the Id attribute is the name of a group of services. If 'no' or not set, the Id attribute refers to another service by name.

**Id** (String, required)
  : The name (not the display name) of a previously installed service or the name of a service group when the Group attribute is set to 'yes'.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)