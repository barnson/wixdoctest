---
custom_edit_url: null
sidebar_position: 32
---
# Chain element
Contains the chain of packages to install.

## Parents
[Bundle](bundle.md)

## Children
* [BundlePackage](bundlepackage.md) 
* [ExePackage](exepackage.md) 
* [MsiPackage](msipackage.md) 
* [MspPackage](msppackage.md) 
* [MsuPackage](msupackage.md) 
* [PackageGroupRef](packagegroupref.md) 
* [RollbackBoundary](rollbackboundary.md) 

## Attributes
**DisableRollback** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the bundle will attempt to rollback packages executed in the chain. If "yes" is specified then when a vital package fails to install only that package will rollback and the chain will stop with the error. The default is "no" which indicates all packages executed during the chain will be rolledback to their previous state when a vital package fails.

**DisableSystemRestore** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the bundle will attempt to create a system restore point when executing the chain. If "yes" is specified then a system restore point will not be created. The default is "no" which indicates a system restore point will be created when the bundle is installed, uninstalled, repaired, modified, etc. If the system restore point cannot be created, the bundle will log the issue and continue.

**ParallelCache** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the bundle will start installing packages while other packages are still being cached. If "yes", packages will start executing when a rollback boundary is encountered. The default is "no" which dictates all packages must be cached before any packages will start to be installed.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)