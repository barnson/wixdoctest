---
custom_edit_url: null
sidebar_position: 126
---
# Launch element
Launch conditions for MSI packages.

## Windows Installer references
[LaunchCondition Table](https://docs.microsoft.com/en-us/windows/win32/msi/launchcondition-table)

## Parents
[Package](package.md), [Fragment](fragment.md)

## Attributes
**Condition** (String, required)
  : The condition expression to be evaluated at install time.

**Message** (String, required)
  : Set the value to the text to display when the condition fails and the installation must be terminated.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)