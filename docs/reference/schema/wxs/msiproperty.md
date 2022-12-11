---
custom_edit_url: null
sidebar_position: 144
---
# MsiProperty element
Allows an MSI property to be set based on the value of a burn engine expression.

## Parents
[MsiPackage](msipackage.md), [MspPackage](msppackage.md)

## Attributes
**Condition** (String)
  : Condition to determine whether to pass the MSI Property. If this evaluates to false, the MSI Property is not passed along.

**Name** (String, required)
  : The name of the MSI property to set. Burn controls the follow MSI properties so they cannot be set with MsiProperty: ACTION, ALLUSERS, REBOOT, REINSTALL, REINSTALLMODE

**Value** (String, required)
  : The value to set the property to. This string is evaluated by the burn engine and can be as simple as a burn engine variable reference or as complex as a full expression.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)