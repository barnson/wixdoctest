---
custom_edit_url: null
toc_max_heading_level: 2
---
# IExtensionData Interface
Interface extensions implement to provide data.
## Methods
| Method | Description |
| ------ | ----------- |
| [GetLibrary(symbolDefinitions)](#getlibrary_symboldefinitions) | Gets the library associated with this extension. |
## Properties
| Property | Description |
| ------ | ----------- |
| [DefaultCulture](#defaultculture) | Gets the optional default culture. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## GetLibrary(symbolDefinitions) Method {#getlibrary_symboldefinitions}
Gets the library associated with this extension.
### Declaration
```cs
public WixToolset.Data.Intermediate GetLibrary(
  WixToolset.Data.ISymbolDefinitionCreator symbolDefinitions
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| symbolDefinitions | WixToolset.Data.ISymbolDefinitionCreator | The symbol definitions to use while loading the library. |
### Return value
`WixToolset.Data.Intermediate` The library for this extension or null if there is no library.
## DefaultCulture Property {#defaultculture}
Gets the optional default culture.
### Declaration
```cs
public string DefaultCulture { get; set; } 
```
