---
custom_edit_url: null
sidebar_position: 2
---
# VsixPackage element (Vs extension)
This element provides the metdata required to install/uninstall a file as a VSIX Package. The VSIX package file will be installed as part of the MSI then passed to the VSIX installer to install the VSIX package. To avoid the duplication, simply use the MSI to install the VSIX package itself.

## Parents
[Component](../wxs/component.md), [File](../wxs/file.md)

## Attributes
**File** (String)
  : Reference to file identifer. This attribute is required when the element is not a child of a File element and is invalid when the element is a child of the File element.

**PackageId** (String, required)
  : Identity of the VSIX package per its internal manifest. If this value is not correct the VSIX package will not correctly uninstall.

**Permanent** (wxs:YesNoTypeUnion)
  : Indicates whether the VSIX package is uninstalled when the parent Component is uninstalled. The default is 'no'.

**Target** (String)
  : Specifies the SKU of Visual Studio in which to register the extension. If no target is specified the extension is registered with all installed SKUs. If the Target attribute is specified the TargetVersion attribute must also be specified. The following is a list of known Visual Studio targets: integratedShell, professional, premium, ultimate, vbExpress, vcExpress, vcsExpress, vwdExpress

**TargetVersion** (wxs:VersionType)
  : Specifies the version of Visual Studio in which to register the extension. This attribute is required if the Target attribute is specified.

**Vital** (wxs:YesNoTypeUnion)
  : Indicates whether failure to install the VSIX package causes the installation to rollback. The default is 'yes'.

**VsixInstallerPathProperty** (String)
  : Optional reference to a Property element that contains the path to the VsixInstaller.exe. By default, the latest VsixInstaller.exe on the machine will be used to install the VSIX package. It is highly recommended that this attribute is *not* used.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/vs.xsd)