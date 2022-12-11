---
custom_edit_url: null
sidebar_position: 178
---
# PermissionEx element
Sets ACLs on File, Registry, or CreateFolder. When under a Registry element, this cannot be used if the Action attribute's value is remove or removeKeyOnInstall. This element is only available when installing with MSI 5.0. For downlevel support, see the PermissionEx element from the WixUtilExtension.

## Windows Installer references
[MsiLockPermissionsEx Table](https://docs.microsoft.com/en-us/windows/win32/msi/msilockpermissionsex-table)

## Attributes
**Condition** (String)
  : Optional condition that controls whether the permissions are applied.

**Id** (String)
  : Primary key used to identify this particular entry. If this is not specified the parent element's Id attribute will be used instead.

**Sddl** (String, required)
  : Security descriptor to apply to parent object.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)