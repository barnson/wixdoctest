---
custom_edit_url: null
toc_max_heading_level: 2
---
# WixUnexpectedFileFormatException Class
Exception when file does not match the expected format.
## Properties
| Property | Description |
| ------ | ----------- |
| [ExpectedFileFormat](#expectedfileformat) | Gets the expected file format. |
| [FileFormat](#fileformat) | Gets the actual file format found in the file. |
| [Path](#path) | Gets the path to the file with unexpected format. |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## ExpectedFileFormat Property {#expectedfileformat}
Gets the expected file format.
### Declaration
```cs
public string ExpectedFileFormat { get; set; } 
```
## FileFormat Property {#fileformat}
Gets the actual file format found in the file.
### Declaration
```cs
public string FileFormat { get; set; } 
```
## Path Property {#path}
Gets the path to the file with unexpected format.
### Declaration
```cs
public string Path { get; set; } 
```
