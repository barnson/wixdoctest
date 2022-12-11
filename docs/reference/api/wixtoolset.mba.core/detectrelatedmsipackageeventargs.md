---
custom_edit_url: null
toc_max_heading_level: 2
---
# DetectRelatedMsiPackageEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectRelatedMsiPackage» 
## Properties
| Property | Description |
| ------ | ----------- |
| [Operation](#operation) | Gets the operation that will be taken on the detected package. |
| [PackageId](#packageid) | Gets the identity of the product's package detected. |
| [PerMachine](#permachine) | Gets whether the detected package is per machine. |
| [ProductCode](#productcode) | Gets the identity of the related package detected. |
| [UpgradeCode](#upgradecode) | Gets the upgrade code of the related package detected. |
| [Version](#version) | Gets the version of the related package detected. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Operation Property {#operation}
Gets the operation that will be taken on the detected package.
### Declaration
```cs
public RelatedOperation Operation { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the product's package detected.
### Declaration
```cs
public string PackageId { get; set; } 
```
## PerMachine Property {#permachine}
Gets whether the detected package is per machine.
### Declaration
```cs
public bool PerMachine { get; set; } 
```
## ProductCode Property {#productcode}
Gets the identity of the related package detected.
### Declaration
```cs
public string ProductCode { get; set; } 
```
## UpgradeCode Property {#upgradecode}
Gets the upgrade code of the related package detected.
### Declaration
```cs
public string UpgradeCode { get; set; } 
```
## Version Property {#version}
Gets the version of the related package detected.
### Declaration
```cs
public string Version { get; set; } 
```
