---
custom_edit_url: null
sidebar_position: 28
---
# BundlePackage element
Describes a single bundle package to install.

## Parents
[Chain](chain.md), [PackageGroup](packagegroup.md)

## Children
* [BundlePackagePayload](bundlepackagepayload.md) 
* [CommandLine](commandline.md) 
* [ExitCode](exitcode.md) 
* [Payload](payload.md) 
* [PayloadGroupRef](payloadgroupref.md) 
* [Provides](provides.md) 

## Attributes
**After** (String)
  : The identifier of another package that this one should be installed after. By default the After attribute is set to the previous sibling package in the Chain or PackageGroup element. If this attribute is specified ensure that a cycle is not created explicitly or implicitly.

**Cache** ([KeepRemoveAlwaysTypeUnion](keepremovealwaystype.md 'Values of this type will either be "always", "keep", or "remove".'))
  : Whether to cache the package. The default is "keep".

**CacheId** (String)
  : The identifier to use when caching the package.

**Compressed** ([YesNoDefaultTypeUnion](yesnodefaulttype.md 'Values of this type will either be "default", "yes", or "no".'))
  : Whether the package payload should be embedded in a container or left as an external payload. Must not be specified if the package payload is given by the *PackagePayload element.

**Description** (String)
  : Specifies the description to place in the bootstrapper application data manifest for the package. By default, ExePackages use the FileName field from the version information, MsiPackages use the ARPCOMMENTS property, and MspPackages use the Description patch metadata property. Other package types must use this attribute to define a description in the bootstrapper application data manifest.

**DisplayName** (String)
  : Specifies the display name to place in the bootstrapper application data manifest for the package. By default, ExePackages use the ProductName field from the version information, MsiPackages use the ProductName property, and MspPackages use the DisplayName patch metadata property. Other package types must use this attribute to define a display name in the bootstrapper application data manifest.

**DownloadUrl** (String)
  : The URL to use to download the package. The following substitutions are supported:  {0} is replaced by the package Id. {1} is replaced by the payload Id. {2} is replaced by the payload file name.  Must not be specified if the package payload is given by the *PackagePayload element.

**Id** (String)
  : Identifier for this package, for ordering and cross-referencing. The default is the Name attribute modified to be suitable as an identifier (i.e. invalid characters are replaced with underscores).

**InstallArguments** (String)
  : The command-line arguments provided to the BundlePackage during install.

**InstallCondition** (String)
  : A condition to evaluate before installing the package. The package will only be installed if the condition evaluates to true. If the condition evaluates to false and the bundle is being installed, repaired, or modified, the package will be uninstalled.

**InstallSize** (String)
  : The size this package will take on disk in bytes after it is installed. By default, the binder will calculate the install size by scanning the package (File table for MSIs, Payloads for EXEs) and use the total for the install size of the package.

**LogPathVariable** (String)
  : Name of a Variable that will hold the path to the log file. An empty value will cause the variable to not be set. The default is "WixBundleLog_[PackageId]" except for MSU packages which default to no logging.

**Name** (String)
  : The destination path and file name for this chain payload. Use this attribute to rename the chain entry point or extract it into a subfolder. The default value is the file name from the SourceFile attribute, if provided. At a minimum, the Name or SourceFile attribute must be specified. This must be a relative path ('\foo' or 'C:\foo' is not allowed). Must not be specified if the package payload is given by the *PackagePayload element.

**Permanent** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the package can be uninstalled. The default is "no".

**RepairArguments** (String)
  : The command-line arguments provided to the BundlePackage during repair. "/repair" is added automatically.

**RepairCondition** (String)
  : A condition that determines during Repair if the package will be repaired by default. This condition can use built-in variables and variables returned by searches.

**RollbackLogPathVariable** (String)
  : Name of a Variable that will hold the path to the log file used during rollback. An empty value will cause the variable to not be set. The default is "WixBundleRollbackLog_[PackageId]" except for MSU packages which default to no logging.

**SourceFile** (String)
  : Location of the package to add to the bundle. The default value is the Name attribute, if provided. At a minimum, the SourceFile or Name attribute must be specified. Must not be specified if the package payload is given by the *PackagePayload element.

**UninstallArguments** (String)
  : The command-line arguments provided to the BundlePackage during uninstall. "/uninstall" is added automatically.

**Visible** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the bundle will be displayed in Programs and Features (also known as Add/Remove Programs). If "yes" is specified the bundle package information will be displayed in Programs and Features. "no" indicates the bundle will not be displayed. If not specified, the default is the value of the Permanent attribute.

**Vital** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the package must succeed for the chain to continue. The default "yes" indicates that if the package fails then the chain will fail and rollback or stop. If "no" is specified then the chain will continue even if the package reports failure.

**PrimaryPackageType** (enumeration)
  : Used by WixInternalUIBootstrapperApplication to determine which package is the primary package. The default value is "default". This attribute's value must be one of the following:
- *default*: This package is used unless there is a package for the runtime machine's architecture.
- *x86*: This package is used when the runtime machine's OS is x86 (IMAGE_FILE_MACHINE_I386).
- *x64*: This package is used when the runtime machine's OS is x64 (IMAGE_FILE_MACHINE_AMD64).
- *arm64*: This package is used when the runtime machine's OS is ARM64 (IMAGE_FILE_MACHINE_ARM64).


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)