---
custom_edit_url: null
toc_max_heading_level: 2
---
# RemoveFileModes Enumeration
Defines values for the InstallMode column of the RemoveFile table.
## Members
| Member | Description |
| ------ | ----------- |
| None | Never remove. |
| OnInstall | Remove when the associated component is being installed (install state = local or source). |
| OnRemove | Remove when the associated component is being removed (install state = absent). |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
