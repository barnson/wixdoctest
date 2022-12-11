---
custom_edit_url: null
sidebar_position: 127
---
# LaunchConditions element
Queries the LaunchCondition table and evaluates each conditional statement recorded there. If any of these conditional statements fail, an error message is displayed to the user and the installation is terminated. The LaunchConditions action is optional. This action is normally the first in the sequence, but the AppSearch Action may be sequenced before the LaunchConditions action. If there are launch conditions that do not apply to all installation modes, the appropriate installation mode property should be used in a conditional expression in the appropriate sequence table. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[LaunchConditions Action](https://docs.microsoft.com/en-us/windows/win32/msi/launchconditions-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md), [AdminUISequence](adminuisequence.md), [AdminExecuteSequence](adminexecutesequence.md)

## See also
[Launch](launch.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)