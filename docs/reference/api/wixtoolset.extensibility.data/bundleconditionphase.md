---
custom_edit_url: null
toc_max_heading_level: 2
---
# BundleConditionPhase Enumeration
The Burn execution phase during which a Condition will be evaluated.
## Members
| Member | Description |
| ------ | ----------- |
| Detect | Condition is evaluated during Detect (ExePackage/@DetectCondition). |
| Execute | Condition is evaluated during Apply (MsiProperty/@Condition). |
| Plan | Condition is evaluated during Plan (ExePackage/@InstallCondition). |
| Shutdown | Condition is evaluated after Apply. |
| Startup | Condition is evaluated by the engine before loading the BootstrapperApplication (Bundle/@Condition). |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
