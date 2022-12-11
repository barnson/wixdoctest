---
custom_edit_url: null
toc_max_heading_level: 2
---
# IWindowsInstallerDecompileResult Interface
The result from decompiling a Windows Installer database.
## Properties
| Property | Description |
| ------ | ----------- |
| [Data](#data) | Decompiled `WindowsInstallerData` . |
| [Document](#document) | Decompiled document. |
| [ExtractedFilePaths](#extractedfilepaths) | Extracted paths. |
| [Platform](#platform) | Decompiled platform. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Data Property {#data}
Decompiled `WindowsInstallerData` .
### Declaration
```cs
public WixToolset.Data.WindowsInstaller.WindowsInstallerData Data { get; set; } 
```
## Document Property {#document}
Decompiled document.
### Declaration
```cs
public System.Xml.Linq.XDocument Document { get; set; } 
```
## ExtractedFilePaths Property {#extractedfilepaths}
Extracted paths.
### Declaration
```cs
public IList<System.String> ExtractedFilePaths { get; set; } 
```
## Platform Property {#platform}
Decompiled platform.
### Declaration
```cs
public System.Nullable<WixToolset.Data.Platform> Platform { get; set; } 
```
