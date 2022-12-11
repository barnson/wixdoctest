---
custom_edit_url: null
toc_max_heading_level: 2
---
# FileAttributes Enumeration
Available values for the Attributes column of the File table.
## Members
| Member | Description |
| ------ | ----------- |
| Checksum | The file contains a valid checksum. A checksum is required to repair a file that has become corrupted. |
| Compressed | The file's source type is compressed. If set, ignore the WordCount summary information property. If neither Noncompressed or Compressed are set, the compression state of the file is specified by the WordCount summary information property. Do not set both Noncompressed and Compressed. |
| Hidden | Hidden. |
| NonCompressed | The file's source type is uncompressed. If set, ignore the WordCount summary information property. If neither Noncompressed nor Compressed are set, the compression state of the file is specified by the WordCount summary information property. Do not set both Noncompressed and Compressed. |
| None | No attributes. |
| PatchAdded | This bit must only be added by a patch and if the file is being added by the patch. |
| ReadOnly | Read-only. |
| System | System. |
| Vital | The file is vital for the proper operation of the component to which it belongs. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
