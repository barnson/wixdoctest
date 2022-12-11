---
custom_edit_url: null
sidebar_position: 230
---
# RMCCPSearch element
Uses file signatures to validate that qualifying products are installed on a system before an upgrade installation is performed. The RMCCPSearch action should be authored into the InstallUISequence table and InstallExecuteSequence table. The installer prevents RMCCPSearch from running in the InstallExecuteSequence sequence if the action has already run in InstallUISequence sequence. The RMCCPSearch action requires the CCP_DRIVE property to be set to the root path on the removable volume that has the installation for any of the qualifying products. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[RMCCPSearch Action](https://docs.microsoft.com/en-us/windows/win32/msi/rmccpsearch-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

## See also
[CCPSearch](ccpsearch.md), [ComplianceCheck](compliancecheck.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)