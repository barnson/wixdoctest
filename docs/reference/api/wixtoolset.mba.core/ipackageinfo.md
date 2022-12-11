---
custom_edit_url: null
toc_max_heading_level: 2
---
# IPackageInfo Interface
Package information from the BA manifest.
## Properties
| Property | Description |
| ------ | ----------- |
| [CacheType](#cachetype) |  |
| [CustomData](#customdata) | Place for the BA to store it's own custom data for this package. |
| [Description](#description) |  |
| [DisplayInternalUICondition](#displayinternaluicondition) |  |
| [DisplayName](#displayname) |  |
| [Id](#id) |  |
| [InstallCondition](#installcondition) |  |
| [Permanent](#permanent) |  |
| [PrereqLicenseFile](#prereqlicensefile) |  |
| [PrereqLicenseUrl](#prereqlicenseurl) |  |
| [PrereqPackage](#prereqpackage) |  |
| [PrimaryPackageType](#primarypackagetype) | See «see P:WixToolset.Mba.Core.IPackageInfo.PrimaryPackageType»  |
| [ProductCode](#productcode) |  |
| [RepairCondition](#repaircondition) |  |
| [Type](#type) |  |
| [UpgradeCode](#upgradecode) |  |
| [Version](#version) |  |
| [Vital](#vital) |  |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CacheType Property {#cachetype}

### Declaration
```cs
public BOOTSTRAPPER_CACHE_TYPE CacheType { get; set; } 
```
## CustomData Property {#customdata}
Place for the BA to store it's own custom data for this package.
### Declaration
```cs
public System.Object CustomData { get; set; } 
```
## Description Property {#description}

### Declaration
```cs
public string Description { get; set; } 
```
## DisplayInternalUICondition Property {#displayinternaluicondition}

### Declaration
```cs
public string DisplayInternalUICondition { get; set; } 
```
## DisplayName Property {#displayname}

### Declaration
```cs
public string DisplayName { get; set; } 
```
## Id Property {#id}

### Declaration
```cs
public string Id { get; set; } 
```
## InstallCondition Property {#installcondition}

### Declaration
```cs
public string InstallCondition { get; set; } 
```
## Permanent Property {#permanent}

### Declaration
```cs
public bool Permanent { get; set; } 
```
## PrereqLicenseFile Property {#prereqlicensefile}

### Declaration
```cs
public string PrereqLicenseFile { get; set; } 
```
## PrereqLicenseUrl Property {#prereqlicenseurl}

### Declaration
```cs
public string PrereqLicenseUrl { get; set; } 
```
## PrereqPackage Property {#prereqpackage}

### Declaration
```cs
public bool PrereqPackage { get; set; } 
```
## PrimaryPackageType Property {#primarypackagetype}
See «see P:WixToolset.Mba.Core.IPackageInfo.PrimaryPackageType» 
### Declaration
```cs
public PrimaryPackageType PrimaryPackageType { get; set; } 
```
## ProductCode Property {#productcode}

### Declaration
```cs
public string ProductCode { get; set; } 
```
## RepairCondition Property {#repaircondition}

### Declaration
```cs
public string RepairCondition { get; set; } 
```
## Type Property {#type}

### Declaration
```cs
public PackageType Type { get; set; } 
```
## UpgradeCode Property {#upgradecode}

### Declaration
```cs
public string UpgradeCode { get; set; } 
```
## Version Property {#version}

### Declaration
```cs
public string Version { get; set; } 
```
## Vital Property {#vital}

### Declaration
```cs
public bool Vital { get; set; } 
```
