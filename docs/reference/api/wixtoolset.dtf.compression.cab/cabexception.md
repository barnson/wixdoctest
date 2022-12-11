---
custom_edit_url: null
toc_max_heading_level: 2
---
# CabException Class
Exception class for cabinet operations.
## Methods
| Method | Description |
| ------ | ----------- |
| [GetObjectData(info, context)](#getobjectdata_info_context) | Sets the SerializationInfo with information about the exception. |
## Properties
| Property | Description |
| ------ | ----------- |
| [Error](#error) | Gets the FCI or FDI cabinet engine error number. |
| [ErrorCode](#errorcode) | Gets the Win32 error code. |
`WixToolset.Dtf.Compression.Cab.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
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
## Error Property {#error}
Gets the FCI or FDI cabinet engine error number.
### Declaration
```cs
public int Error { get; set; } 
```
## ErrorCode Property {#errorcode}
Gets the Win32 error code.
### Declaration
```cs
public int ErrorCode { get; set; } 
```
