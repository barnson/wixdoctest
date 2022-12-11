---
custom_edit_url: null
toc_max_heading_level: 2
---
# EndSessionReasons Enumeration
One or more reasons why the application is requested to be closed or is being closed.
## Members
| Member | Description |
| ------ | ----------- |
| CloseApplication | The application is using a file that must be replaced, the system is being serviced, or system resources are exhausted. |
| Critical | The application is forced to shut down. |
| Logoff | The user is logging off. |
| Unknown | The system is shutting down or restarting (it is not possible to determine which event is occurring). |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
