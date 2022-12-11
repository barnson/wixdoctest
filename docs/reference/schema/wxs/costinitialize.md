---
custom_edit_url: null
sidebar_position: 51
---
# CostInitialize element
Initiates the internal installation costing process. Any standard or custom actions that affect costing should be sequenced before the CostInitialize action. Call the FileCost action immediately following the CostInitialize action. Then call the CostFinalize action following the CostInitialize action to make all final cost calculations available to the installer through the Component table. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[CostInitialize Action](https://docs.microsoft.com/en-us/windows/win32/msi/costinitialize-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md), [AdminUISequence](adminuisequence.md), [AdminExecuteSequence](adminexecutesequence.md), [AdvertiseExecuteSequence](advertiseexecutesequence.md)

## See also
[FileCost](filecost.md), [CostFinalize](costfinalize.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)