---
custom_edit_url: null
sidebar_position: 36
---
# CommandLine element
Describes additional, conditional command-line arguments for an ExePackage or BundlePackage.

## Parents
[ExePackage](exepackage.md), [BundlePackage](bundlepackage.md)

## Attributes
**Condition** (String)
  : The condition that controls whether the command-line arguments specified in the InstallArgument, UninstallArgument, or RepairArgument attributes are appended to the command line passed to the package. Which attribute is used depends on the action being applied to the package. For example, when the package is being installed, the InstallArgument attribute value is appended to the command line when the package is executed.

**InstallArgument** (String)
  : Additional command-line arguments to apply during package installation if Condition is true.

**RepairArgument** (String)
  : Additional command-line arguments to apply during package repair if Condition is true.

**UninstallArgument** (String)
  : Additional command-line arguments to apply during package uninstallation if Condition is true.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)