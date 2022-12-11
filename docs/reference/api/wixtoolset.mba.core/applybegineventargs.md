---
custom_edit_url: null
toc_max_heading_level: 2
---
# ApplyBeginEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ApplyBegin» 
## Properties
| Property | Description |
| ------ | ----------- |
| [PhaseCount](#phasecount) | Gets the number of phases that the engine will go through in apply. There are currently two possible phases: cache and execute. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PhaseCount Property {#phasecount}
Gets the number of phases that the engine will go through in apply. There are currently two possible phases: cache and execute.
### Declaration
```cs
public int PhaseCount { get; set; } 
```
