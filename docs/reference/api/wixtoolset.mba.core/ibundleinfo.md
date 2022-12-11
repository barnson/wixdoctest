---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBundleInfo Interface
BA manifest data.
## Methods
| Method | Description |
| ------ | ----------- |
| [AddRelatedBundleAsPackage(e)](#addrelatedbundleaspackage_e) | Adds a related bundle as a package. |
| [AddUpdateBundleAsPackage(e)](#addupdatebundleaspackage_e) | Adds an update bundle as a package. |
## Properties
| Property | Description |
| ------ | ----------- |
| [LogVariable](#logvariable) |  |
| [Name](#name) |  |
| [OverridableVariables](#overridablevariables) |  |
| [Packages](#packages) |  |
| [PerMachine](#permachine) |  |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## AddRelatedBundleAsPackage(e) Method {#addrelatedbundleaspackage_e}
Adds a related bundle as a package.
### Declaration
```cs
public IPackageInfo AddRelatedBundleAsPackage(
  DetectRelatedBundleEventArgs e
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| e | DetectRelatedBundleEventArgs |  |
### Return value
`IPackageInfo` The created «see T:WixToolset.Mba.Core.IPackageInfo» .
## AddUpdateBundleAsPackage(e) Method {#addupdatebundleaspackage_e}
Adds an update bundle as a package.
### Declaration
```cs
public IPackageInfo AddUpdateBundleAsPackage(
  SetUpdateCompleteEventArgs e
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| e | SetUpdateCompleteEventArgs |  |
### Return value
`IPackageInfo` The created «see T:WixToolset.Mba.Core.IPackageInfo» .
## LogVariable Property {#logvariable}

### Declaration
```cs
public string LogVariable { get; set; } 
```
## Name Property {#name}

### Declaration
```cs
public string Name { get; set; } 
```
## OverridableVariables Property {#overridablevariables}

### Declaration
```cs
public IOverridableVariables OverridableVariables { get; set; } 
```
## Packages Property {#packages}

### Declaration
```cs
public System.Collections.Generic.IDictionary<System.String,WixToolset.Mba.Core.IPackageInfo> Packages { get; set; } 
```
## PerMachine Property {#permachine}

### Declaration
```cs
public bool PerMachine { get; set; } 
```
