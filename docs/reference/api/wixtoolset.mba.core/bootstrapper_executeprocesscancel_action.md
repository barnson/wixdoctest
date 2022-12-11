---
custom_edit_url: null
toc_max_heading_level: 2
---
# BOOTSTRAPPER_EXECUTEPROCESSCANCEL_ACTION Enumeration
The available actions for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecuteProcessCancel» .
## Members
| Member | Description |
| ------ | ----------- |
| Abandon | Instructs the engine to stop waiting for the process to exit. The package is immediately considered to have failed with ERROR_INSTALL_USEREXIT. The engine will never rollback the package. |
| Wait | Instructs the engine to wait for the process to exit. Once the process has exited, the package is considered to have failed with ERROR_INSTALL_USEREXIT. This allows the engine to rollback the package if necessary. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
