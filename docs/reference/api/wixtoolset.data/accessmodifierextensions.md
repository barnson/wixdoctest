---
custom_edit_url: null
toc_max_heading_level: 2
---
# AccessModifierExtensions Class
Extensions for converting `AccessModifier` to and from strings optimally.
## Methods
| Method | Description |
| ------ | ----------- |
| [AsAccessModifier(access)](#asaccessmodifier_access) | Converts a string to an `AccessModifier` . |
| [AsString(access)](#asstring_access) | Converts an `AccessModifier` to a string. |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## AsAccessModifier(access) Method {#asaccessmodifier_access}
Converts a string to an `AccessModifier` .
### Declaration
```cs
public static AccessModifier AsAccessModifier(
  string access
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| access | string | String value to convert. |
### Return value
`AccessModifier` Converted `AccessModifier` .
## AsString(access) Method {#asstring_access}
Converts an `AccessModifier` to a string.
### Declaration
```cs
public static string AsString(
  AccessModifier access
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| access | AccessModifier | AccessModifier value to convert. |
### Return value
`string` Converted string.
