---
custom_edit_url: null
sidebar_position: 50
---
# CostFinalize element
Ends the internal installation costing process begun by the CostInitialize action. Any standard or custom actions that affect costing should be sequenced before the CostInitialize action. Call the FileCost action immediately following the CostInitialize action and then call the CostFinalize action to make all final cost calculations available to the installer through the Component table. The CostFinalize action must be executed before starting any user interface sequence which allows the user to view or modify Feature table selections or directories. The CostFinalize action queries the Condition table to determine which features are scheduled to be installed. Costing is done for each component in the Component table. The CostFinalize action also verifies that all the target directories are writable before allowing the installation to continue. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[CostFinalize Action](https://docs.microsoft.com/en-us/windows/win32/msi/costfinalize-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md), [AdminUISequence](adminuisequence.md), [AdminExecuteSequence](adminexecutesequence.md), [AdvertiseExecuteSequence](advertiseexecutesequence.md)

## See also
[CostInitialize](costinitialize.md), [FileCost](filecost.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)