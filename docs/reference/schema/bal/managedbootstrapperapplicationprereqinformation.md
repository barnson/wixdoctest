---
custom_edit_url: null
sidebar_position: 2
---
# ManagedBootstrapperApplicationPrereqInformation element (Bal extension)
Adds license information for a prereq package, should only be used when unable to add the license attributes to the package directly.

## Parents
[Bundle](../wxs/bundle.md), [Fragment](../wxs/fragment.md)

## Attributes
**LicenseFile** (String)
  : Source file of the license. May not be used with LicenseUrl.

**LicenseUrl** (String)
  : Source url of the license. May not be used with LicenseFile.

**PackageId** (String, required)
  : Id of the target package.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/bal.xsd)