---
custom_edit_url: null
toc_max_heading_level: 2
---
# MessageResult Enumeration
Specifies a return status value for message handlers. These values are returned by «see M:WixToolset.Dtf.WindowsInstaller.Session.Message(WixToolset.Dtf.WindowsInstaller.InstallMessage,WixToolset.Dtf.WindowsInstaller.Record)» , «see T:WixToolset.Dtf.WindowsInstaller.ExternalUIHandler» , and «see M:WixToolset.Dtf.WindowsInstaller.IEmbeddedUI.ProcessMessage(WixToolset.Dtf.WindowsInstaller.InstallMessage,WixToolset.Dtf.WindowsInstaller.Record,WixToolset.Dtf.WindowsInstaller.MessageButtons,WixToolset.Dtf.WindowsInstaller.MessageIcon,WixToolset.Dtf.WindowsInstaller.MessageDefaultButton)» .
## Members
| Member | Description |
| ------ | ----------- |
| Abort | IDABORT |
| Cancel | IDCANCEL |
| Error | An error was found in the message handler. |
| Ignore | IDIGNORE |
| No | IDNO |
| None | No action was taken. |
| OK | IDOK |
| Retry | IDRETRY |
| Yes | IDYES |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
