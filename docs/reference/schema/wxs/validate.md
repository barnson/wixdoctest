---
custom_edit_url: null
sidebar_position: 285
---
# Validate element
Sets information in the patch transform that determines if the transform applies to an installed product and what errors should be ignored when applying the patch transform.

## Parents
[PatchBaseline](patchbaseline.md)

## Remarks
<p>A transform contains the differences between the target product and the upgraded product. When a transform or a patch (which contains transforms) is applied, the following properties of the installed product are validated against the properties of the target product stored in a transform.</p>
<ul>
  <li>ProductCode</li>
  <li>ProductLanguage</li>
  <li>ProductVersion</li>
  <li>UpgradeCode</li>
</ul>
<p>Windows Installer simply validates that the ProductCode, ProductLanguage, and UpgradeCode of an installed product are equivalent to those propeties of the target product used to create the transform; however, the ProductVersion can be validated with a greater range of comparisons.</p>
<p>You can compare up to the first three fields of the ProductVersion. Changes to the fourth field are not validated and are useful for small updates. You can also choose how to compare the target ProductVersion used to create the transform with the installed ProductVersion. For example, while the default value of 'Equals' is recommended, if you wanted a minor upgrade patch to apply to the target ProductVersion and all older products with the same ProductCode, you would use 'LesserOrEqual'.</p>


## Attributes
**IgnoreAddExistingRow** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Ignore errors when adding existing rows. The default is 'yes'.

**IgnoreAddExistingTable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Ignore errors when adding existing tables. The default is 'yes'.

**IgnoreChangingCodePage** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Ignore errors when changing the database code page. The default is 'no'.

**IgnoreDeleteMissingRow** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Ignore errors when deleting missing rows. The default is 'yes'.

**IgnoreDeleteMissingTable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Ignore errors when deleting missing tables. The default is 'yes'.

**IgnoreUpdateMissingRow** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Ignore errors when updating missing rows. The default is 'yes'.

**ProductId** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Requires that the installed ProductCode match the target ProductCode used to create the transform. The default is 'yes'.

**ProductLanguage** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Requires that the installed ProductLanguage match the target ProductLanguage used to create the transform. The default is 'no'.

**ProductVersion** (enumeration)
  : Determines how many fields of the installed ProductVersion to compare. See remarks for more information. The default is 'Update'. This attribute's value must be one of the following:
- *Major*: Checks the major version.
- *Minor*: Checks the major and minor versions.
- *Update*: Checks the major, minor, and update versions.

**ProductVersionOperator** (enumeration)
  : Determines how the installed ProductVersion is compared to the target ProductVersion used to create the transform. See remarks for more information. The default is 'Equal'. This attribute's value must be one of the following:
- *Lesser*: Installed ProductVersion < target ProductVersion.
- *LesserOrEqual*: Installed ProductVersion <= target ProductVersion.
- *Equal*: Installed ProductVersion = target ProductVersion.
- *GreaterOrEqual*: Installed ProductVersion >= target ProductVersion.
- *Greater*: Installed ProductVersion > target ProductVersion.

**UpgradeCode** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Requires that the installed UpgradeCode match the target UpgradeCode used to create the transform. The default is 'yes'.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)