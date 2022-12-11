---
custom_edit_url: null
sidebar_position: 133
---
# MajorUpgrade element
Simplifies authoring for major upgrades, including support for preventing downgrades.  The parent Package element must have valid UpgradeCode and Version attributes.  When the FindRelatedProducts action detects a related product installed on the system, it appends the product code to the property named WIX_UPGRADE_DETECTED. After the FindRelatedProducts action is run, the value of the WIX_UPGRADE_DETECTED property is a list of product codes, separated by semicolons (;), detected on the system.

## Parents
[Package](package.md)

## Attributes
**AllowDowngrades** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When set to no (the default), products with lower version numbers are blocked from installing when a product with a higher version is installed; the DowngradeErrorMessage attribute must also be specified.  When set to yes, any version can be installed over any other version.

**AllowSameVersionUpgrades** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When set to no (the default), installing a product with the same version and upgrade code (but different product code) is allowed and treated by MSI as two products. When set to yes, WiX sets the msidbUpgradeAttributesVersionMaxInclusive attribute, which tells MSI to treat a product with the same version as a major upgrade.  This is useful when two product versions differ only in the fourth version field. MSI specifically ignores that field when comparing product versions, so two products that differ only in the fourth version field are the same product and need this attribute set to yes to be detected.  Note that because MSI ignores the fourth product version field, setting this attribute to yes also allows downgrades when the first three product version fields are identical. For example, product version 1.0.0.1 will "upgrade" 1.0.0.2998 because they're seen as the same version (1.0.0). That could reintroduce serious bugs so the safest choice is to change the first three version fields and omit this attribute to get the default of no.  This attribute cannot be "yes" when AllowDowngrades is also "yes" -- AllowDowngrades already allows two products with the same version number to upgrade each other.

**Disallow** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When set to yes, products with higer version numbers are blocked from installing when a product with a lower version is installed; the UpgradeErrorMessage attribute must also be specified.  When set to no (the default), any version can be installed over any lower version.

**DisallowUpgradeErrorMessage** (String)
  : The message displayed if users try to install a product with a higer version number when a product with a lower version is installed. Used only when Disallow is yes.

**DowngradeErrorMessage** (String)
  : The message displayed if users try to install a product with a lower version number when a product with a higher version is installed. Used only when AllowDowngrades is no (the default).

**IgnoreLanguage** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When set to yes, the Upgrade table rows will match any product with the same UpgradeCode.  When set to no (the default), the Upgrade table rows will match only products with the same UpgradeCode and ProductLanguage.

**IgnoreRemoveFailure** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When set to yes, failures removing the installed product during the upgrade will be ignored.  When set to no (the default), failures removing the installed product during the upgrade will be considered a failure and, depending on the scheduling, roll back the upgrade.

**MigrateFeatures** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When set to yes (the default), the MigrateFeatureStates standard action will set the feature states of the upgrade product to those of the installed product.  When set to no, the installed features have no effect on the upgrade installation.

**RemoveFeatures** (String)
  : A formatted string that contains the list of features to remove from the installed product. The default is to remove all features. Note that if you use formatted property values that evaluate to an empty string, no features will be removed; only omitting this attribute defaults to removing all features.

**Schedule** (enumeration)
  : Determines the scheduling of the RemoveExistingProducts standard action, which is when the installed product is removed. The default is "afterInstallValidate" which removes the installed product entirely before installing the upgrade product. It's slowest but gives the most flexibility in changing components and features in the upgrade product.  For more information, see RemoveExistingProducts. This attribute's value must be one of the following:
- *afterInstallValidate*: (Default) Schedules RemoveExistingProducts after the InstallValidate standard action. This scheduling removes the installed product entirely before installing the upgrade product. It's slowest but gives the most flexibility in changing components and features in the upgrade product. Note that if the installation of the upgrade product fails, the machine will have neither version installed.
- *afterInstallInitialize*: Schedules RemoveExistingProducts after the InstallInitialize standard action. This is similar to the afterInstallValidate scheduling, but if the installation of the upgrade product fails, Windows Installer also rolls back the removal of the installed product -- in other words, reinstalls it.
- *afterInstallExecute*: Schedules RemoveExistingProducts between the InstallExecute and InstallFinalize standard actions. This scheduling installs the upgrade product "on top of" the installed product then lets RemoveExistingProducts uninstall any components that don't also exist in the upgrade product. Note that this scheduling requires strict adherence to the component rules because it relies on component reference counts to be accurate during installation of the upgrade product and removal of the installed product. For more information, see  Bob Arnson's blog post "Paying for Upgrades" for details. If installation of the upgrade product fails, Windows Installer also rolls back the removal of the installed product -- in other words, reinstalls it.
- *afterInstallExecuteAgain*: Schedules RemoveExistingProducts between the InstallExecuteAgain and InstallFinalize standard actions. This is identical to the afterInstallExecute scheduling but after the InstallExecuteAgain standard action instead of InstallExecute.
- *afterInstallFinalize*: Schedules RemoveExistingProducts after the InstallFinalize standard action. This is similar to the afterInstallExecute and afterInstallExecuteAgain schedulings but takes place outside the installation transaction so if installation of the upgrade product fails, Windows Installer does not roll back the removal of the installed product, so the machine will have both versions installed.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)