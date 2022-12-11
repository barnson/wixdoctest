---
custom_edit_url: null
sidebar_position: 153
---
# ODBCDriver element
ODBCDriver for a Component

## Windows Installer references
[ODBCDriver Table](https://docs.microsoft.com/en-us/windows/win32/msi/odbcdriver-table)

## Parents
[File](file.md), [Component](component.md)

## Children
* [ODBCDataSource](odbcdatasource.md) 
* [Property](property.md) 

## Attributes
**File** (String)
  : Required if not found as child of File element

**Id** (String, required)
  : Identifier for the driver.

**Name** (String, required)
  : Name for the driver.

**SetupFile** (String)
  : Required if not found as child of File element or different from File attribute above


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)