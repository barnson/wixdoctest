---
custom_edit_url: null
toc_max_heading_level: 2
---
# ReinstallModes Enumeration
Specifies the reinstall mode for «see M:WixToolset.Dtf.WindowsInstaller.Installer.ReinstallFeature(System.String,System.String,WixToolset.Dtf.WindowsInstaller.ReinstallModes)» or «see M:WixToolset.Dtf.WindowsInstaller.Installer.ReinstallProduct(System.String,WixToolset.Dtf.WindowsInstaller.ReinstallModes)» .
## Members
| Member | Description |
| ------ | ----------- |
| FileEqualVersion | Reinstall if file is missing, or equal or older version. |
| FileExact | Reinstall if file is missing, or not exact version. |
| FileMissing | Reinstall only if file is missing. |
| FileOlderVersion | Reinstall if file is missing, or older version. |
| FileReplace | Reinstall all files, regardless of version. |
| FileVerify | Checksum executables, reinstall if missing or corrupt. |
| MachineData | Insure required machine reg entries. |
| Package | Use re-cache source install package. |
| Shortcut | Validate shortcuts items. |
| UserData | Insure required user reg entries. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
