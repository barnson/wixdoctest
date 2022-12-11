---
custom_edit_url: null
sidebar_position: 22
---
# PerfCounterManifest element (Util extension)
Used to install Perfmon Counter Manifests. Note that this functionality cannot be used with major upgrades that are scheduled after the InstallExecute, InstallExecuteAgain, or InstallFinalize actions. For more information on major upgrade scheduling, see [RemoveExistingProducts Action](https://learn.microsoft.com/en-us/windows/win32/msi/removeexistingproducts-action).

## Parents
[File](../wxs/file.md)

## Attributes
**ResourceFileDirectory** (String)
  : The directory that holds the resource file of the providers in the perfmon counter manifest. Often the resource file path cannot be determined until setup time. Put the directory here and during perfmon manifest registrtion the path will be updated in the registry. If not specified, Perfmon will look for the resource file in the same directory of the perfmon counter manifest file.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)