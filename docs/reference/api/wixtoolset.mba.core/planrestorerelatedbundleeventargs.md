---
custom_edit_url: null
toc_max_heading_level: 2
---
# PlanRestoreRelatedBundleEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanRestoreRelatedBundle» 
## Properties
| Property | Description |
| ------ | ----------- |
| [BundleId](#bundleid) | Gets the identity of the bundle to plan for. |
| [RecommendedState](#recommendedstate) | Gets the recommended requested state for the bundle. |
| [State](#state) | Gets or sets the requested state for the bundle. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## BundleId Property {#bundleid}
Gets the identity of the bundle to plan for.
### Declaration
```cs
public string BundleId { get; set; } 
```
## RecommendedState Property {#recommendedstate}
Gets the recommended requested state for the bundle.
### Declaration
```cs
public RequestState RecommendedState { get; set; } 
```
## State Property {#state}
Gets or sets the requested state for the bundle.
### Declaration
```cs
public RequestState State { get; set; } 
```
