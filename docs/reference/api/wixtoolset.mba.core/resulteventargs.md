---
custom_edit_url: null
toc_max_heading_level: 2
---
# ResultEventArgs Class
Base class for «see T:System.EventArgs» classes that must return a «see P:WixToolset.Mba.Core.ResultEventArgs.Result» .
## Properties
| Property | Description |
| ------ | ----------- |
| [Recommendation](#recommendation) | Gets the recommended «see P:WixToolset.Mba.Core.ResultEventArgs.Result» of the operation. |
| [Result](#result) | Gets or sets the «see P:WixToolset.Mba.Core.ResultEventArgs.Result» of the operation. This is passed back to the engine. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Recommendation Property {#recommendation}
Gets the recommended «see P:WixToolset.Mba.Core.ResultEventArgs.Result» of the operation.
### Declaration
```cs
public Result Recommendation { get; set; } 
```
## Result Property {#result}
Gets or sets the «see P:WixToolset.Mba.Core.ResultEventArgs.Result» of the operation. This is passed back to the engine.
### Declaration
```cs
public Result Result { get; set; } 
```
