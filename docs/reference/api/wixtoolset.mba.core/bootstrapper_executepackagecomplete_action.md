---
custom_edit_url: null
toc_max_heading_level: 2
---
# BOOTSTRAPPER_EXECUTEPACKAGECOMPLETE_ACTION Enumeration
The available actions for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecutePackageComplete» .
## Members
| Member | Description |
| ------ | ----------- |
| Ignore | Instructs the engine to ignore non-vital package failures and continue with the install. Ignored if hrStatus is a success or the package is vital. |
| None |  |
| Restart | Instructs the engine to stop processing the chain and restart. The engine will launch again after the machine is restarted. |
| Retry | Instructs the engine to try the execution of the package again. Ignored if hrStatus is a success. |
| Suspend | Instructs the engine to stop processing the chain and suspend the current state. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
