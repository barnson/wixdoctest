---
custom_edit_url: null
sidebar_position: 284
---
# UpgradeVersion element


## Windows Installer references
[Upgrade Table](https://docs.microsoft.com/en-us/windows/win32/msi/upgrade-table)

## Parents
[Upgrade](upgrade.md)

## Attributes
**ExcludeLanguages** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "yes" to detect all languages, excluding the languages listed in the Language attribute.

**IgnoreRemoveFailure** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "yes" to continue installation upon failure to remove a product or application.

**IncludeMaximum** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "yes" to make the range of versions detected include the value specified in Maximum.

**IncludeMinimum** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "no" to make the range of versions detected exclude the value specified in Minimum. This attribute is "yes" by default.

**Language** (String)
  : Specifies the set of languages detected by FindRelatedProducts. Enter a list of numeric language identifiers (LANGID) separated by commas (,). Leave this value null to specify all languages. Set ExcludeLanguages to "yes" in order detect all languages, excluding the languages listed in this value.

**Maximum** (String)
  : Specifies the upper boundary of the range of product versions detected by FindRelatedProducts.

**MigrateFeatures** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "yes" to migrate feature states from upgraded products by enabling the logic in the MigrateFeatureStates action.

**Minimum** (String)
  : Specifies the lower bound on the range of product versions to be detected by FindRelatedProducts.

**OnlyDetect** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set to "yes" to detect products and applications but do not uninstall.

**Property** (String, required)
  : When the FindRelatedProducts action detects a related product installed on the system, it appends the product code to the property specified in this field. Windows Installer documentation for the Upgrade table states that the property specified in this field must be a public property and must be added to the SecureCustomProperties property. WiX automatically appends the property specified in this field to the SecureCustomProperties property when creating an MSI. Each UpgradeVersion must have a unique Property value. After the FindRelatedProducts action is run, the value of this property is a list of product codes, separated by semicolons (;), detected on the system.

**RemoveFeatures** (String)
  : The installer sets the REMOVE property to features specified in this column. The features to be removed can be determined at run time. The Formatted string entered in this field must evaluate to a comma-delimited list of feature names. For example: [Feature1],[Feature2],[Feature3]. No features are removed if the field contains formatted text that evaluates to an empty string. The installer sets REMOVE=ALL only if the Remove field is empty.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)