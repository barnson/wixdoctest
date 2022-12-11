---
custom_edit_url: null
sidebar_position: 119
---
# InstallUISequence element


## Windows Installer references
[InstallUISequence Table](https://docs.microsoft.com/en-us/windows/win32/msi/installuisequence-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [UI](ui.md)

## Children
* [AppSearch](appsearch.md) : Uses file signatures to search for existing versions of products.
* [CCPSearch](ccpsearch.md) : Uses file signatures to validate that qualifying products are installed on a system before an upgrade installation is performed.
* [CostFinalize](costfinalize.md) : Ends the internal installation costing process begun by the CostInitialize action.
* [CostInitialize](costinitialize.md) : Initiates the internal installation costing process.
* [Custom](custom.md) : Use to sequence a custom action.
* [ExecuteAction](executeaction.md) : Initiates the execution sequence.
* [FileCost](filecost.md) : Initiates dynamic costing of standard installation actions.
* [FindRelatedProducts](findrelatedproducts.md) : Runs through each record of the Upgrade table in sequence and compares the upgrade code, product version, and language in each row to products installed on the system.
* [IsolateComponents](isolatecomponents.md) : Installs a copy of a component (commonly a shared DLL) into a private location for use by a specific application (typically an .exe).
* [LaunchConditions](launchconditions.md) : Queries the LaunchCondition table and evaluates each conditional statement recorded there.
* [MigrateFeatureStates](migratefeaturestates.md) : Used for upgrading or installing over an existing application.
* [ResolveSource](resolvesource.md) : Determines the location of the source and sets the SourceDir property if the source has not been resolved yet.
* [RMCCPSearch](rmccpsearch.md) : Uses file signatures to validate that qualifying products are installed on a system before an upgrade installation is performed.
* [ScheduleReboot](schedulereboot.md) : Prompts the user to restart the system at the end of installation. Not fixed sequence.
* [Show](show.md) : Displays a Dialog.
* [ValidateProductID](validateproductid.md) : Sets the ProductID property to the full product identifier.

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)