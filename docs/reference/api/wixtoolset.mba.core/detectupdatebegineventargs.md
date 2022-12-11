---
custom_edit_url: null
toc_max_heading_level: 2
---
# DetectUpdateBeginEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectUpdateBegin» 
## Properties
| Property | Description |
| ------ | ----------- |
| [Skip](#skip) | Whether to skip checking for bundle updates. |
| [UpdateLocation](#updatelocation) | Gets the identity of the bundle to detect. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Skip Property {#skip}
Whether to skip checking for bundle updates.
### Declaration
```cs
public bool Skip { get; set; } 
```
## UpdateLocation Property {#updatelocation}
Gets the identity of the bundle to detect.
### Declaration
```cs
public string UpdateLocation { get; set; } 
```
