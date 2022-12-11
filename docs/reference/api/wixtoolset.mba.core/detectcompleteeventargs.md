---
custom_edit_url: null
toc_max_heading_level: 2
---
# DetectCompleteEventArgs Class
Additional arguments used when the detection phase has completed.
## Properties
| Property | Description |
| ------ | ----------- |
| [EligibleForCleanup](#eligibleforcleanup) | Indicates whether the engine will uninstall the bundle if shutdown without running Apply. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## EligibleForCleanup Property {#eligibleforcleanup}
Indicates whether the engine will uninstall the bundle if shutdown without running Apply.
### Declaration
```cs
public bool EligibleForCleanup { get; set; } 
```
