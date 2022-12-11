---
custom_edit_url: null
toc_max_heading_level: 2
---
# PlanRelatedBundleTypeEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanRelatedBundleType» 
## Properties
| Property | Description |
| ------ | ----------- |
| [BundleId](#bundleid) | Gets the identity of the bundle to plan for. |
| [RecommendedType](#recommendedtype) | Gets the recommended plan type for the bundle. |
| [Type](#type) | Gets or sets the plan type for the bundle. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## BundleId Property {#bundleid}
Gets the identity of the bundle to plan for.
### Declaration
```cs
public string BundleId { get; set; } 
```
## RecommendedType Property {#recommendedtype}
Gets the recommended plan type for the bundle.
### Declaration
```cs
public RelatedBundlePlanType RecommendedType { get; set; } 
```
## Type Property {#type}
Gets or sets the plan type for the bundle.
### Declaration
```cs
public RelatedBundlePlanType Type { get; set; } 
```
