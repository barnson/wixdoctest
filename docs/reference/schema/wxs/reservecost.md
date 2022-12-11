---
custom_edit_url: null
sidebar_position: 228
---
# ReserveCost element
Disk cost to reserve in a folder for running locally and/or from source.

## Windows Installer references
[ReserveCost Table](https://docs.microsoft.com/en-us/windows/win32/msi/reservecost-table)

## Parents
[Component](component.md)

## Attributes
**Directory** (String)
  : Adds the amount of disk space specified in RunFromSource or RunLocal to the volume cost of the device containing the directory. If this attribute is not set, it will default to the directory of parent component.

**Id** (String, required)
  : A primary key that uniquely identifies this ReserveCost entry.

**RunFromSource** (Integer, required)
  : The number of bytes of disk space to reserve if the component is installed to run from source.

**RunLocal** (Integer, required)
  : The number of bytes of disk space to reserve if the component is installed to run locally.

**Subdirectory** (String)
  : This attribute defines one or more directories below the directory referenced by the Directory attribute to add cost to.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)