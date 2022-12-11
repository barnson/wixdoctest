---
custom_edit_url: null
toc_max_heading_level: 2
---
# DetectMsiFeatureEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectMsiFeature» 
## Properties
| Property | Description |
| ------ | ----------- |
| [FeatureId](#featureid) | Gets the identity of the feature detected. |
| [PackageId](#packageid) | Gets the identity of the feature's package detected. |
| [State](#state) | Gets the detected feature state. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## FeatureId Property {#featureid}
Gets the identity of the feature detected.
### Declaration
```cs
public string FeatureId { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the feature's package detected.
### Declaration
```cs
public string PackageId { get; set; } 
```
## State Property {#state}
Gets the detected feature state.
### Declaration
```cs
public FeatureState State { get; set; } 
```
