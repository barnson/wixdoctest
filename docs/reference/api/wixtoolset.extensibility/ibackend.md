---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBackend Interface
Interface all backends implement.
## Methods
| Method | Description |
| ------ | ----------- |
| [Bind(context)](#bind_context) | Bind the intermediate into the final output. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Bind(context) Method {#bind_context}
Bind the intermediate into the final output.
### Declaration
```cs
public Data.IBindResult Bind(
  Data.IBindContext context
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| context | Data.IBindContext | Bind context. |
### Return value
`Data.IBindResult` Result of the bind operation.
