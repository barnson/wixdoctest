---
custom_edit_url: null
toc_max_heading_level: 2
---
# IWixBranding Interface
WiX branding interface.
## Methods
| Method | Description |
| ------ | ----------- |
| [GetCreatingApplication()](#getcreatingapplication_nop) | Gets the value for CreatingApplication field (MSI Summary Information Stream). |
| [ReplacePlaceholders(original, assembly)](#replaceplaceholders_original_assembly) | Replaces branding placeholders in original string. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## GetCreatingApplication() Method {#getcreatingapplication_nop}
Gets the value for CreatingApplication field (MSI Summary Information Stream).
### Declaration
```cs
public string GetCreatingApplication
```
### Return value
`string` String for creating application.
## ReplacePlaceholders(original, assembly) Method {#replaceplaceholders_original_assembly}
Replaces branding placeholders in original string.
### Declaration
```cs
public string ReplacePlaceholders(
  string original,
  System.Reflection.Assembly assembly
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| original | string | Original string containing placeholders to replace. |
| assembly | System.Reflection.Assembly | Optional assembly with branding information, if not specified core branding is used. |
