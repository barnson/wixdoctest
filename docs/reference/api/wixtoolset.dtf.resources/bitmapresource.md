---
custom_edit_url: null
toc_max_heading_level: 2
---
# BitmapResource Class
A subclass of Resource which provides specific methods for manipulating the resource data.
## Methods
| Method | Description |
| ------ | ----------- |
| [ReadFromFile(path)](#readfromfile_path) | Reads the bitmap from a .bmp file. |
### Remarks
The resource is of type «see P:WixToolset.Dtf.Resources.ResourceType.Bitmap» (RT_GROUPICON).
`WixToolset.Dtf.Resources.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## ReadFromFile(path) Method {#readfromfile_path}
Reads the bitmap from a .bmp file.
### Declaration
```cs
public void ReadFromFile(
  string path
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| path | string | Path to a bitmap file (.bmp). |
