---
custom_edit_url: null
sidebar_position: 171
---
# PatchMetadata element
Properties about the patch to be placed in the PatchMetadata table.

## Windows Installer references
[MsiPatchMetadata Table](https://docs.microsoft.com/en-us/windows/win32/msi/msipatchmetadata-table)

## Parents
[PatchCreation](patchcreation.md)

## Children
* [CustomProperty](customproperty.md) 
* [OptimizeCustomActions](optimizecustomactions.md) (no more than 1) : Indicates whether custom actions can be skipped when applying the patch.

## Attributes
**AllowRemoval** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'), required)
  : Whether this is an uninstallable patch.

**Classification** (String, required)
  : Category of updates. Recommended values are Critical Update, Hotfix, Security Rollup, Security Update, Service Pack, Update, Update Rollup.

**CreationTimeUTC** (String)
  : Creation time of the .msp file in the form mm-dd-yy HH:MM (month-day-year hour:minute).

**Description** (String, required)
  : Description of the patch.

**DisplayName** (String, required)
  : A title for the patch that is suitable for public display. In Add/Remove Programs from XP SP2 on.

**ManufacturerName** (String, required)
  : Name of the manufacturer.

**MinorUpdateTargetRTM** (String)
  : Indicates that the patch targets the RTM version of the product or the most recent major upgrade patch. Author this optional property in minor update patches that contain sequencing information to indicate that the patch removes all patches up to the RTM version of the product, or up to the most recent major upgrade patch. This property is available beginning with Windows Installer 3.1.

**MoreInfoURL** (String, required)
  : A URL that provides information specific to this patch. In Add/Remove Programs from XP SP2 on.

**OptimizedInstallMode** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If this attribute is set to 'yes' in all the patches to be applied in a transaction, the application of the patch is optimized if possible. Available beginning with Windows Installer 3.1.

**TargetProductName** (String, required)
  : Name of the application or target product suite.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)