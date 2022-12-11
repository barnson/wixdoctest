---
custom_edit_url: null
sidebar_position: 231
---
# RollbackBoundary element
Describes a rollback boundary in the chain.

## Parents
[Chain](chain.md), [PackageGroup](packagegroup.md)

## Attributes
**Id** (String)
  : Identifier for this rollback boundary, for ordering and cross-referencing. If this attribute is not provided a stable identifier will be generated.

**LogPathVariable** (String)
  : Name of a Variable that will hold the path to the log file when the rollback boundary is a MSI package transaction. An empty value will cause the variable to not be set. The default is "WixBundleLog_[RollbackBoundaryId]".

**Transaction** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the rollback boundary is wrapped in an MSI transaction. The default is "no". Only MsiPackages and MspPackages may be inside of a rollback boundary with Transaction set to "yes".

**Vital** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the rollback boundary aborts the chain. The default "yes" indicates that if the rollback boundary is encountered then the chain will fail and rollback or stop. If "no" is specified then the chain should continue successfuly at the next rollback boundary.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)