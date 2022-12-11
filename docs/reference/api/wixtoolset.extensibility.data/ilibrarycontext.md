---
custom_edit_url: null
toc_max_heading_level: 2
---
# ILibraryContext Interface
Context provided during library creation operations.
## Properties
| Property | Description |
| ------ | ----------- |
| [BindFiles](#bindfiles) | Indicates whether files should be bound into the library. |
| [BindPaths](#bindpaths) | Collection of bindpaths used to bind files. |
| [CancellationToken](#cancellationtoken) | Cancellation token. |
| [Extensions](#extensions) | Collection of extensions used during creation of library. |
| [IntermediateFolder](#intermediatefolder) | Intermediate folder. |
| [Intermediates](#intermediates) | Collection of intermediates to include in the library. |
| [LibraryId](#libraryid) | Identifier of the library. |
| [Localizations](#localizations) | Collection of localization files to use in the library. |
| [OutputPath](#outputpath) | Output path. |
| [ServiceProvider](#serviceprovider) | Service provider. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## BindFiles Property {#bindfiles}
Indicates whether files should be bound into the library.
### Declaration
```cs
public bool BindFiles { get; set; } 
```
## BindPaths Property {#bindpaths}
Collection of bindpaths used to bind files.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.IBindPath> BindPaths { get; set; } 
```
## CancellationToken Property {#cancellationtoken}
Cancellation token.
### Declaration
```cs
public System.Threading.CancellationToken CancellationToken { get; set; } 
```
## Extensions Property {#extensions}
Collection of extensions used during creation of library.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.ILibrarianExtension> Extensions { get; set; } 
```
## IntermediateFolder Property {#intermediatefolder}
Intermediate folder.
### Declaration
```cs
public string IntermediateFolder { get; set; } 
```
## Intermediates Property {#intermediates}
Collection of intermediates to include in the library.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Data.Intermediate> Intermediates { get; set; } 
```
## LibraryId Property {#libraryid}
Identifier of the library.
### Declaration
```cs
public string LibraryId { get; set; } 
```
## Localizations Property {#localizations}
Collection of localization files to use in the library.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Data.Localization> Localizations { get; set; } 
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
