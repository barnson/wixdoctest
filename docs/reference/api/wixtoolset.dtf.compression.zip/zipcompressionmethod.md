---
custom_edit_url: null
toc_max_heading_level: 2
---
# ZipCompressionMethod Enumeration
Identifies the compression method or "algorithm" used for a single file within a zip archive.
## Members
| Member | Description |
| ------ | ----------- |
| BZip2 | The file is compressed using the BZIP2 algorithm. |
| Deflate | The file is Deflated; the most common and widely-compatible form of zip compression. |
| Deflate64 | The file is Deflated using the enhanced Deflate64 method. |
| Implode | The file is Imploded |
| Lzma | The file is compressed using the LZMA algorithm. |
| Ppmd | The file is compressed using the PPMd algorithm. |
| Reduce1 | The file is Reduced with compression factor 1 |
| Reduce2 | The file is Reduced with compression factor 2 |
| Reduce3 | The file is Reduced with compression factor 3 |
| Reduce4 | The file is Reduced with compression factor 4 |
| Shrink | The file is Shrunk |
| Store | The file is stored (no compression) |
### Remarks
Proprietary zip implementations may define additional compression methods outside of those included here.
`WixToolset.Dtf.Compression.Zip.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
