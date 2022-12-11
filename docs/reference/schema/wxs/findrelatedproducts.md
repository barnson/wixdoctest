---
custom_edit_url: null
sidebar_position: 100
---
# FindRelatedProducts element
Runs through each record of the Upgrade table in sequence and compares the upgrade code, product version, and language in each row to products installed on the system. When FindRelatedProducts detects a correspondence between the upgrade information and an installed product, it appends the product code to the property specified in the ActionProperty column of the UpgradeTable. The FindRelatedProducts action only runs the first time the product is installed. The FindRelatedProducts action does not run during maintenance mode or uninstallation. FindRelatedProducts should be authored into the InstallUISequence table and InstallExecuteSequence tables. The installer prevents FindRelatedProducts from running in InstallExecuteSequence if the action has already run in InstallUISequence. The FindRelatedProducts action must come before the MigrateFeatureStates action and the RemoveExistingProducts action. The condition for this action may be specified in the element's inner text.

## Windows Installer references
[FindRelatedProducts Action](https://docs.microsoft.com/en-us/windows/win32/msi/findrelatedproducts-action)

## Parents
[InstallUISequence](installuisequence.md), [InstallExecuteSequence](installexecutesequence.md)

## See also
[Upgrade](upgrade.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)