---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBindContext Interface
Bind context.
## Properties
| Property | Description |
| ------ | ----------- |
| [BindPaths](#bindpaths) | Bind paths used during resolution. |
| [CabbingThreadCount](#cabbingthreadcount) | Counnt of threads to use in cabbing. |
| [CabCachePath](#cabcachepath) | Cabinet cache path. |
| [CancellationToken](#cancellationtoken) | Cancellation token. |
| [DefaultCompressionLevel](#defaultcompressionlevel) | Default compression level. |
| [DelayedFields](#delayedfields) | Delayed fields that need to be resolved again. |
| [ExpectedEmbeddedFiles](#expectedembeddedfiles) | Embedded files to extract. |
| [Extensions](#extensions) | Binder extensions. |
| [FileSystemExtensions](#filesystemextensions) | File system extensions. |
| [IntermediateFolder](#intermediatefolder) | Intermedaite folder. |
| [IntermediateRepresentation](#intermediaterepresentation) | Intermediate representation to bind. |
| [OutputPath](#outputpath) | Output path to bind to. |
| [PdbPath](#pdbpath) | Output path for PDB. |
| [PdbType](#pdbtype) | Type of PDB to create. |
| [ResolvedCodepage](#resolvedcodepage) | Codepage from resolve. |
| [ResolvedLcid](#resolvedlcid) | LCID from resolve. |
| [ResolvedSummaryInformationCodepage](#resolvedsummaryinformationcodepage) | Summary information codepage from resolve. |
| [ServiceProvider](#serviceprovider) | Service provider. |
| [SuppressLayout](#suppresslayout) | Skip creation of output. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## BindPaths Property {#bindpaths}
Bind paths used during resolution.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.IBindPath> BindPaths { get; set; } 
```
## CabbingThreadCount Property {#cabbingthreadcount}
Counnt of threads to use in cabbing.
### Declaration
```cs
public int CabbingThreadCount { get; set; } 
```
## CabCachePath Property {#cabcachepath}
Cabinet cache path.
### Declaration
```cs
public string CabCachePath { get; set; } 
```
## CancellationToken Property {#cancellationtoken}
Cancellation token.
### Declaration
```cs
public System.Threading.CancellationToken CancellationToken { get; set; } 
```
## DefaultCompressionLevel Property {#defaultcompressionlevel}
Default compression level.
### Declaration
```cs
public System.Nullable<WixToolset.Data.CompressionLevel> DefaultCompressionLevel { get; set; } 
```
## DelayedFields Property {#delayedfields}
Delayed fields that need to be resolved again.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.IDelayedField> DelayedFields { get; set; } 
```
## ExpectedEmbeddedFiles Property {#expectedembeddedfiles}
Embedded files to extract.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.IExpectedExtractFile> ExpectedEmbeddedFiles { get; set; } 
```
## Extensions Property {#extensions}
Binder extensions.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.IBinderExtension> Extensions { get; set; } 
```
## FileSystemExtensions Property {#filesystemextensions}
File system extensions.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.IFileSystemExtension> FileSystemExtensions { get; set; } 
```
## IntermediateFolder Property {#intermediatefolder}
Intermedaite folder.
### Declaration
```cs
public string IntermediateFolder { get; set; } 
```
## IntermediateRepresentation Property {#intermediaterepresentation}
Intermediate representation to bind.
### Declaration
```cs
public WixToolset.Data.Intermediate IntermediateRepresentation { get; set; } 
```
## OutputPath Property {#outputpath}
Output path to bind to.
### Declaration
```cs
public string OutputPath { get; set; } 
```
## PdbPath Property {#pdbpath}
Output path for PDB.
### Declaration
```cs
public string PdbPath { get; set; } 
```
## PdbType Property {#pdbtype}
Type of PDB to create.
### Declaration
```cs
public WixToolset.Data.PdbType PdbType { get; set; } 
```
## ResolvedCodepage Property {#resolvedcodepage}
Codepage from resolve.
### Declaration
```cs
public System.Nullable<System.Int32> ResolvedCodepage { get; set; } 
```
## ResolvedLcid Property {#resolvedlcid}
LCID from resolve.
### Declaration
```cs
public System.Nullable<System.Int32> ResolvedLcid { get; set; } 
```
## ResolvedSummaryInformationCodepage Property {#resolvedsummaryinformationcodepage}
Summary information codepage from resolve.
### Declaration
```cs
public System.Nullable<System.Int32> ResolvedSummaryInformationCodepage { get; set; } 
```
## ServiceProvider Property {#serviceprovider}
Service provider.
### Declaration
```cs
public System.IServiceProvider ServiceProvider { get; set; } 
```
## SuppressLayout Property {#suppresslayout}
Skip creation of output.
### Declaration
```cs
public bool SuppressLayout { get; set; } 
```
