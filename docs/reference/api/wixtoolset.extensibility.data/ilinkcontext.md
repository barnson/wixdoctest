---
custom_edit_url: null
toc_max_heading_level: 2
---
# ILinkContext Interface
Context provided during linking.
## Properties
| Property | Description |
| ------ | ----------- |
| [CancellationToken](#cancellationtoken) | Cancellation token. |
| [ExpectedOutputType](#expectedoutputtype) | Expected output type. |
| [ExtensionData](#extensiondata) | Collection of extension data to use during linking. |
| [Extensions](#extensions) | Collection of extensions to use during linking. |
| [IntermediateFolder](#intermediatefolder) | Intermediate folder. |
| [Intermediates](#intermediates) | Collection of intermediates to link. |
| [OutputPath](#outputpath) | Output path. |
| [ServiceProvider](#serviceprovider) | Service provider. |
| [SymbolDefinitionCreator](#symboldefinitioncreator) | Symbol definition creator used to load extension data. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CancellationToken Property {#cancellationtoken}
Cancellation token.
### Declaration
```cs
public System.Threading.CancellationToken CancellationToken { get; set; } 
```
## ExpectedOutputType Property {#expectedoutputtype}
Expected output type.
### Declaration
```cs
public WixToolset.Data.OutputType ExpectedOutputType { get; set; } 
```
## ExtensionData Property {#extensiondata}
Collection of extension data to use during linking.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.IExtensionData> ExtensionData { get; set; } 
```
## Extensions Property {#extensions}
Collection of extensions to use during linking.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.ILinkerExtension> Extensions { get; set; } 
```
## IntermediateFolder Property {#intermediatefolder}
Intermediate folder.
### Declaration
```cs
public string IntermediateFolder { get; set; } 
```
## Intermediates Property {#intermediates}
Collection of intermediates to link.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Data.Intermediate> Intermediates { get; set; } 
```
## OutputPath Property {#outputpath}
Output path.
### Declaration
```cs
public string OutputPath { get; set; } 
```
## ServiceProvider Property {#serviceprovider}
Service provider.
### Declaration
```cs
public System.IServiceProvider ServiceProvider { get; set; } 
```
## SymbolDefinitionCreator Property {#symboldefinitioncreator}
Symbol definition creator used to load extension data.
### Declaration
```cs
public WixToolset.Data.ISymbolDefinitionCreator SymbolDefinitionCreator { get; set; } 
```
