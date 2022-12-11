---
custom_edit_url: null
toc_max_heading_level: 2
---
# LaunchApprovedExeCompleteEventArgs Class
Additional arguments passed by the engine after it finished trying to launch the preapproved executable.
## Properties
| Property | Description |
| ------ | ----------- |
| [ProcessId](#processid) | Gets the ProcessId of the process that was launched. This is only valid if the status reports success. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## ProcessId Property {#processid}
Gets the ProcessId of the process that was launched. This is only valid if the status reports success.
### Declaration
```cs
public int ProcessId { get; set; } 
```
