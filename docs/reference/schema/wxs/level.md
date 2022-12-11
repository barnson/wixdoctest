---
custom_edit_url: null
sidebar_position: 128
---
# Level element
Feature levels for MSI packages.

## Windows Installer references
[Condition Table](https://docs.microsoft.com/en-us/windows/win32/msi/condition-table)

## Parents
[Feature](feature.md)

## Attributes
**Condition** (String, required)
  : The condition expression to be evaluated at install time. When true the Feature level is set to the Value.

**Value** (Integer, required)
  : Allows modifying the level of a Feature based on the result of the condition.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)