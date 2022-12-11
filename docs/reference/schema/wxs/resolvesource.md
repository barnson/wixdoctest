---
custom_edit_url: null
sidebar_position: 229
---
# ResolveSource element
Determines the location of the source and sets the SourceDir property if the source has not been resolved yet. Special actions don't have a built-in sequence number and thus must appear relative to another action. The suggested way to do this is by using the Before or After attribute. InstallExecute and InstallExecuteAgain can optionally appear anywhere between InstallInitialize and InstallFinalize.

## Windows Installer references
[ResolveSource Action](https://docs.microsoft.com/en-us/windows/win32/msi/resolvesource-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md), [AdminExecuteSequence](adminexecutesequence.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)