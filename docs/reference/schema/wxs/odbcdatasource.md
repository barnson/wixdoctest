---
custom_edit_url: null
sidebar_position: 152
---
# ODBCDataSource element
ODBCDataSource for a Component

## Windows Installer references
[ODBCDataSource Table](https://docs.microsoft.com/en-us/windows/win32/msi/odbcdatasource-table)

## Parents
[ODBCDriver](odbcdriver.md), [Component](component.md)

## Children
* [Property](property.md) 

## Attributes
**DriverName** (String)
  : Required if not found as child of ODBCDriver element

**Id** (String, required)
  : Identifier of the data source.

**KeyPath** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set 'yes' to force this file to be key path for parent Component

**Name** (String, required)
  : Name for the data source.

**Registration** (enumeration, required)
  : Scope for which the data source should be registered. This attribute's value must be one of the following:
- *machine*: Data source is registered per machine.
- *user*: Data source is registered per user.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)