---
custom_edit_url: null
toc_max_heading_level: 2
---
# LocalizedControl Class

## Methods
| Method | Description |
| ------ | ----------- |
| [GetKey()](#getkey_nop) | Get key for a localized control. |
| [GetKey(dialog, control)](#getkey_dialog_control) | Get key for a localized control. |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## GetKey() Method {#getkey_nop}
Get key for a localized control.
### Declaration
```cs
public string GetKey
```
### Return value
`string` The localized control id.
## GetKey(dialog, control) Method {#getkey_dialog_control}
Get key for a localized control.
### Declaration
```cs
public static string GetKey(
  string dialog,
  string control
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| dialog | string | The optional id of the control's dialog. |
| control | string | The id of the control. |
### Return value
`string` The localized control id.
