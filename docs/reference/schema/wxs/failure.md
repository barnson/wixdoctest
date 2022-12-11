---
custom_edit_url: null
sidebar_position: 89
---
# Failure element
Failure action for a ServiceConfigFailureActions element.

## Parents
[ServiceConfigFailureActions](serviceconfigfailureactions.md)

## Attributes
**Action** (String, required)
  : Specifies the action to take when the service fails. Valid values are "none", "restartComputer", "restartService", "runCommand" or a Formatted property that resolves to "0" (for "none"), "1" (for "restartService"), "2" (for "restartComputer") or "3" (for "runCommand").

**Delay** (String, required)
  : Specifies the time in milliseconds to wait before performing the value from the Action attribute.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)