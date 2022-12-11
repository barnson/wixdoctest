---
custom_edit_url: null
sidebar_position: 233
---
# ScheduleReboot element
Prompts the user to restart the system at the end of installation. Special actions don't have a built-in sequence number and thus must appear relative to another action. The suggested way to do this is by using the Before or After attribute. InstallExecute and InstallExecuteAgain can optionally appear anywhere between InstallInitialize and InstallFinalize.

## Windows Installer references
[ScheduleReboot Action](https://docs.microsoft.com/en-us/windows/win32/msi/schedulereboot-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)