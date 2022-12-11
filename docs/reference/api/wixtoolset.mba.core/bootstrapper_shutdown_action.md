---
custom_edit_url: null
toc_max_heading_level: 2
---
# BOOTSTRAPPER_SHUTDOWN_ACTION Enumeration
The available actions for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.Shutdown» .
## Members
| Member | Description |
| ------ | ----------- |
| None |  |
| ReloadBootstrapper | Instructs the engine to unload the bootstrapper application and restart the engine which will load the bootstrapper application again. Typically used to switch from a native bootstrapper application to a managed one. |
| Restart | Instructs the engine to restart. The engine will not launch again after the machine is rebooted. Ignored if reboot was already initiated by «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecutePackageComplete» . |
| SkipCleanup | Opts out of the engine behavior of trying to uninstall itself when no non-permanent packages are installed. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
