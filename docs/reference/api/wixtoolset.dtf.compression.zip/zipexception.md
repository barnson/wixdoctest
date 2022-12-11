---
custom_edit_url: null
toc_max_heading_level: 2
---
# ZipException Class
Exception class for zip operations.
## Methods
| Method | Description |
| ------ | ----------- |
| [GetObjectData(info, context)](#getobjectdata_info_context) | Sets the SerializationInfo with information about the exception. |
`WixToolset.Dtf.Compression.Zip.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## GetObjectData(info, context) Method {#getobjectdata_info_context}
Sets the SerializationInfo with information about the exception.
### Declaration
```cs
public void GetObjectData(
  System.Runtime.Serialization.SerializationInfo info,
  System.Runtime.Serialization.StreamingContext context
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| info | System.Runtime.Serialization.SerializationInfo | The SerializationInfo that holds the serialized object data about the exception being thrown. |
| context | System.Runtime.Serialization.StreamingContext | The StreamingContext that contains contextual information about the source or destination. |
