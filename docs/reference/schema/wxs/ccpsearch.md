---
custom_edit_url: null
sidebar_position: 31
---
# CCPSearch element
Uses file signatures to validate that qualifying products are installed on a system before an upgrade installation is performed. The CCPSearch action should be authored into the InstallUISequence table and InstallExecuteSequence table. The installer prevents the CCPSearch action from running in the InstallExecuteSequence sequence if the action has already run in InstallUISequence sequence. The CCPSearch action must come before the RMCCPSearch action. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[CCPSearch Action](https://docs.microsoft.com/en-us/windows/win32/msi/ccpsearch-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

## See also
[RMCCPSearch](rmccpsearch.md), [ComplianceCheck](compliancecheck.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)