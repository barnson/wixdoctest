---
custom_edit_url: null
sidebar_position: 112
---
# InstallExecuteAgain element
Runs a script containing all operations spooled since either the start of the installation or the last InstallExecute action, or InstallExecuteAgain action. Should only be used after InstallExecute. Special actions don't have a built-in sequence number and thus must appear relative to another action. The suggested way to do this is by using the Before or After attribute. InstallExecute and InstallExecuteAgain can optionally appear anywhere between InstallInitialize and InstallFinalize.

## Windows Installer references
[InstallExecuteAgain Action](https://docs.microsoft.com/en-us/windows/win32/msi/installexecuteagain-action)

## Parents
[InstallExecuteSequence](installexecutesequence.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)