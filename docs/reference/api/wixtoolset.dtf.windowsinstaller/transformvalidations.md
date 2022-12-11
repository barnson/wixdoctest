---
custom_edit_url: null
toc_max_heading_level: 2
---
# TransformValidations Enumeration
Transform validation flags available for «see M:WixToolset.Dtf.WindowsInstaller.Database.CreateTransformSummaryInfo(WixToolset.Dtf.WindowsInstaller.Database,System.String,WixToolset.Dtf.WindowsInstaller.TransformErrors,WixToolset.Dtf.WindowsInstaller.TransformValidations)» .
## Members
| Member | Description |
| ------ | ----------- |
| Language | Default language must match base database. |
| MajorVersion | Check major version only. |
| MinorVersion | Check major and minor versions only. |
| NewEqualBaseVersion | Installed version = base version. |
| NewGreaterBaseVersion | Installed version {'>'} base version. |
| NewGreaterEqualBaseVersion | Installed version {'>'}= base version. |
| NewLessBaseVersion | Installed version {'<'} base version. |
| NewLessEqualBaseVersion | Installed version {'<'}= base version. |
| None | Validate no properties. |
| Product | Product must match base database. |
| UpdateVersion | Check major, minor, and update versions. |
| UpgradeCode | UpgradeCode must match base database. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
