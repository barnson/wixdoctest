---
custom_edit_url: null
sidebar_position: 2
---
# AdminUISequence element


## Windows Installer references
[AdminUISequence Table](https://docs.microsoft.com/en-us/windows/win32/msi/adminuisequence-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [UI](ui.md)

## Children
* [CostFinalize](costfinalize.md) : Ends the internal installation costing process begun by the CostInitialize action.
* [CostInitialize](costinitialize.md) : Initiates the internal installation costing process.
* [Custom](custom.md) : Use to sequence a custom action.
* [ExecuteAction](executeaction.md) : Initiates the execution sequence.
* [FileCost](filecost.md) : Initiates dynamic costing of standard installation actions.
* [InstallAdminPackage](installadminpackage.md) : Copies the product database to the administrative installation point.
* [InstallFiles](installfiles.md) : Copies files specified in the File table from the source directory to the destination directory.
* [InstallFinalize](installfinalize.md) : Marks the end of a sequence of actions that change the system.
* [InstallInitialize](installinitialize.md) : Marks the beginning of a sequence of actions that change the system.
* [InstallValidate](installvalidate.md) : Verifies that all costed volumes have enough space for the installation.
* [LaunchConditions](launchconditions.md) : Queries the LaunchCondition table and evaluates each conditional statement recorded there.
* [Show](show.md) 

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)