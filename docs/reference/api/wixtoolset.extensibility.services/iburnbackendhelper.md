---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBurnBackendHelper Interface
Interface provided to help Burn backend extensions.
## Methods
| Method | Description |
| ------ | ----------- |
| [AddBootstrapperApplicationData(xml)](#addbootstrapperapplicationdata_xml) | Adds the given XML to the BootstrapperApplicationData manifest. |
| [AddBootstrapperApplicationData(symbol, symbolIdIsIdAttribute)](#addbootstrapperapplicationdata_symbol_symbolidisidattribute) | Adds an XML element for the given symbol to the BootstrapperApplicationData manifest. The symbol's name is used for the element's name. All of the symbol's fields are used for the element's attributes. |
| [AddBundleExtensionData(extensionId, xml)](#addbundleextensiondata_extensionid_xml) | Adds the given XML to the BundleExtensionData manifest for the given bundle extension. |
| [AddBundleExtensionData(extensionId, symbol, symbolIdIsIdAttribute)](#addbundleextensiondata_extensionid_symbol_symbolidisidattribute) | Adds an XML element for the given symbol to the BundleExtensionData manifest for the given bundle extension. The symbol's name is used for the element's name. All of the symbol's fields are used for the element's attributes. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## AddBootstrapperApplicationData(xml) Method {#addbootstrapperapplicationdata_xml}
Adds the given XML to the BootstrapperApplicationData manifest.
### Declaration
```cs
public void AddBootstrapperApplicationData(
  string xml
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| xml | string | A valid XML fragment. |
## AddBootstrapperApplicationData(symbol, symbolIdIsIdAttribute) Method {#addbootstrapperapplicationdata_symbol_symbolidisidattribute}
Adds an XML element for the given symbol to the BootstrapperApplicationData manifest. The symbol's name is used for the element's name. All of the symbol's fields are used for the element's attributes.
### Declaration
```cs
public void AddBootstrapperApplicationData(
  WixToolset.Data.IntermediateSymbol symbol,
  bool symbolIdIsIdAttribute
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| symbol | WixToolset.Data.IntermediateSymbol | The symbol to create the element from. |
| symbolIdIsIdAttribute | bool | If true and the symbol has an Id, then an Id attribute is created with a value of the symbol's Id. |
## AddBundleExtensionData(extensionId, xml) Method {#addbundleextensiondata_extensionid_xml}
Adds the given XML to the BundleExtensionData manifest for the given bundle extension.
### Declaration
```cs
public void AddBundleExtensionData(
  string extensionId,
  string xml
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| extensionId | string | The bundle extension's id. |
| xml | string | A valid XML fragment. |
## AddBundleExtensionData(extensionId, symbol, symbolIdIsIdAttribute) Method {#addbundleextensiondata_extensionid_symbol_symbolidisidattribute}
Adds an XML element for the given symbol to the BundleExtensionData manifest for the given bundle extension. The symbol's name is used for the element's name. All of the symbol's fields are used for the element's attributes.
### Declaration
```cs
public void AddBundleExtensionData(
  string extensionId,
  WixToolset.Data.IntermediateSymbol symbol,
  bool symbolIdIsIdAttribute
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| extensionId | string | The bundle extension's id. |
| symbol | WixToolset.Data.IntermediateSymbol | The symbol to create the element from. |
| symbolIdIsIdAttribute | bool | If true and the symbol has an Id, then an Id attribute is created with a value of the symbol's Id. |
