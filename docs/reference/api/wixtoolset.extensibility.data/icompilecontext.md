---
custom_edit_url: null
toc_max_heading_level: 2
---
# ICompileContext Interface
Context provided to the compiler.
## Properties
| Property | Description |
| ------ | ----------- |
| [CancellationToken](#cancellationtoken) | Cancellation token to abort cancellation. |
| [CompilationId](#compilationid) | Unique identifier for the compilation. |
| [Extensions](#extensions) | Set of extensions provided to the compiler. |
| [IntermediateFolder](#intermediatefolder) | Intermediate folder. |
| [IsCurrentPlatform64Bit](#iscurrentplatform64bit) | Calculates whether the target platform for the compilation is 64-bit or not. |
| [OutputPath](#outputpath) | Output path. |
| [Platform](#platform) | Gets or sets the platform which the compiler will use when defaulting 64-bit attributes and elements. |
| [ServiceProvider](#serviceprovider) | Service provider made available to the compiler and its extensions. |
| [Source](#source) | Source document being compiled. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CancellationToken Property {#cancellationtoken}
Cancellation token to abort cancellation.
### Declaration
```cs
public System.Threading.CancellationToken CancellationToken { get; set; } 
```
## CompilationId Property {#compilationid}
Unique identifier for the compilation.
### Declaration
```cs
public string CompilationId { get; set; } 
```
## Extensions Property {#extensions}
Set of extensions provided to the compiler.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.ICompilerExtension> Extensions { get; set; } 
```
## IntermediateFolder Property {#intermediatefolder}
Intermediate folder.
### Declaration
```cs
public string IntermediateFolder { get; set; } 
```
## IsCurrentPlatform64Bit Property {#iscurrentplatform64bit}
Calculates whether the target platform for the compilation is 64-bit or not.
### Declaration
```cs
public bool IsCurrentPlatform64Bit { get; set; } 
```
## OutputPath Property {#outputpath}
Output path.
### Declaration
```cs
public string OutputPath { get; set; } 
```
## Platform Property {#platform}
Gets or sets the platform which the compiler will use when defaulting 64-bit attributes and elements.
### Declaration
```cs
public WixToolset.Data.Platform Platform { get; set; } 
```
## ServiceProvider Property {#serviceprovider}
Service provider made available to the compiler and its extensions.
### Declaration
```cs
public System.IServiceProvider ServiceProvider { get; set; } 
```
## Source Property {#source}
Source document being compiled.
### Declaration
```cs
public System.Xml.Linq.XDocument Source { get; set; } 
```
