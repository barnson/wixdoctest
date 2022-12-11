---
custom_edit_url: null
toc_max_heading_level: 2
---
# InstallUIOptions Enumeration
Level of the installation user interface, specified with «see M:WixToolset.Dtf.WindowsInstaller.Installer.SetInternalUI(WixToolset.Dtf.WindowsInstaller.InstallUIOptions)» .
## Members
| Member | Description |
| ------ | ----------- |
| Basic | Simple progress and error handling. |
| Default | Uses Default UI level. |
| EndDialog | When combined with another value, the installer displays a modal dialog box at the end of a successful installation or if there has been an error. No dialog box is displayed if the user cancels. |
| Full | Authored UI with wizards, progress, and errors. |
| HideCancel | When combined with the «see F:WixToolset.Dtf.WindowsInstaller.InstallUIOptions.Basic» value, the installer does not display the cancel button in the progress dialog. |
| NoChange | Does not change UI level. |
| ProgressOnly | When combined with the «see F:WixToolset.Dtf.WindowsInstaller.InstallUIOptions.Basic» value, the installer displays progress dialog boxes but does not display any modal dialog boxes or error dialog boxes. |
| Reduced | Authored UI, wizard dialogs suppressed. |
| Silent | Silent installation. |
| SourceResolutionOnly | Forces display of the source resolution dialog even if the UI is otherwise silent. |
| UacOnly | [MSI 5.0] Forces display of the UAC dialog even if the UI is otherwise silent. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
