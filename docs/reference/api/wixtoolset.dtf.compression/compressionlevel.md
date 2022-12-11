---
custom_edit_url: null
toc_max_heading_level: 2
---
# CompressionLevel Enumeration
Specifies the compression level ranging from minimum compresion to maximum compression, or no compression at all.
## Members
| Member | Description |
| ------ | ----------- |
| Max | Maximum compression; slowest. |
| Min | Minimum compression; fastest. |
| None | Do not compress files, only store. |
| Normal | A compromize between speed and compression efficiency. |
### Remarks
Although only four values are enumerated, any integral value between «see F:WixToolset.Dtf.Compression.CompressionLevel.Min» and «see F:WixToolset.Dtf.Compression.CompressionLevel.Max» can also be used.
`WixToolset.Dtf.Compression.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
