---
custom_edit_url: null
toc_max_heading_level: 2
---
# InstallMode Enumeration
Specifies the install mode for «see M:WixToolset.Dtf.WindowsInstaller.Installer.ProvideComponent(System.String,System.String,System.String,WixToolset.Dtf.WindowsInstaller.InstallMode)» or «see M:WixToolset.Dtf.WindowsInstaller.Installer.ProvideQualifiedComponent(System.String,System.String,WixToolset.Dtf.WindowsInstaller.InstallMode,System.String)» .
## Members
| Member | Description |
| ------ | ----------- |
| Default | Provide the component and perform any installation necessary to provide the component. |
| Existing | Provide the component only if the feature exists. |
| NoDetection | Only check that the component is registered, without verifying that the key file of the component exists. |
| NoSourceResolution | Provide the component only if the feature's installation state is «see F:WixToolset.Dtf.WindowsInstaller.InstallState.Local» . |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
