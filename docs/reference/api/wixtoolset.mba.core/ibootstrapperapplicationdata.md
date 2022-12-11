---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBootstrapperApplicationData Interface
Interface for BootstrapperApplicationData.xml.
## Properties
| Property | Description |
| ------ | ----------- |
| [BADataFile](#badatafile) | The BootstrapperApplicationData.xml file. |
| [Bundle](#bundle) | The BA manifest. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## BADataFile Property {#badatafile}
The BootstrapperApplicationData.xml file.
### Declaration
```cs
public System.IO.FileInfo BADataFile { get; set; } 
```
## Bundle Property {#bundle}
The BA manifest.
### Declaration
```cs
public IBundleInfo Bundle { get; set; } 
```
