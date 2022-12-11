---
custom_edit_url: null
toc_max_heading_level: 2
---
# INSTALLUILEVEL Enumeration
From msi.h https://docs.microsoft.com/en-us/windows/win32/api/msi/nf-msi-msisetinternalui
## Members
| Member | Description |
| ------ | ----------- |
| Basic | simple progress and error handling |
| Default | default UI is used |
| EndDialog | display success/failure dialog at end of install |
| Full | authored UI with wizards, progress, errors |
| HideCancel | do not display the cancel button in basic UI |
| NoChange | UI level is unchanged |
| None | completely silent installation |
| ProgressOnly | display only progress dialog |
| Reduced | authored UI, wizard dialogs suppressed |
| SourceResOnly | force display of source resolution even if quiet |
| UacOnly | show UAC prompt even if quiet Can only be used if on Windows Installer 5.0 or later |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
